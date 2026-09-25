# Project Status & Handoff Tracking (`PROGRESS.md`)

## 1. Where We Stand
- **Core System**: Self-contained client-side web application (`index.html`) implementing the Non-API Model & Quota Comparator.
- **Model Coverage**: 22 model variations across Google, Anthropic, and OpenAI.
- **Accurate 2026 Limits**: 1M+ context limits and 128k output boundaries verified for late 2026 frontier models.
- **Comprehensive Vibe Coding Evals**: Displaying 6 industry standard scores for all models with hover tooltips and dynamic highlighting:
  - **SWE-bench Verified**: Autonomous issue resolution.
  - **Chatbot Arena (Coding)**: Human-rated preference / vibes.
  - **Aider Code Editing**: Refactoring pass rate.
  - **Instruction Following (IFEval)**: Measures AI obedience and prevents laziness.
  - **Context Recall (NIAH)**: Measures massive context memory retention.
  - **LiveCodeBench**: Measures novel problem solving against memorization.
- **Comparison Engine**: Head-to-Head view automatically calculates the highest score across compared models and badges the winner.
- **Persistence**: `localStorage` automatic saving and state restoration on page load.

---

## 2. What's Left (Next Priorities)
- **Export / Share Feature**: Allow users to export or share their configured simulator settings.
- **Visual Charting**: Optional canvas-based breakdown showing proportion of context vs output vs thinking tokens per task.
- **Custom Plan Override**: Allow power users to input custom token ceilings.

---

## 3. Context & Gotchas
- **Zero-Build UI**: Pure HTML5/JS/Tailwind without a build step for portability. Tooltips rely on native HTML `title` attributes with Tailwind `cursor-help` for maximum cross-browser reliability. Comparison highlighting is computed dynamically on each dropdown change.
