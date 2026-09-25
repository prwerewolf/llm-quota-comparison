# Project Status & Handoff Tracking (`PROGRESS.md`)

## 1. Where We Stand
- **Core System**: Self-contained client-side web application (`index.html`) implementing the Non-API Model & Quota Comparator.
- **Model Coverage**: 22 model variations across Google, Anthropic, and OpenAI.
- **Accurate 2026 Limits**: 1M+ context limits and 128k output boundaries verified for late 2026 frontier models.
- **Vibe Coding Benchmarks Added**: Displaying industry standard agentic scores for all models:
  - **SWE-bench Verified**: Measures autonomous GitHub issue resolution.
  - **LMSYS Chatbot Arena (Coding)**: Human-rated preference / Elo vibes.
  - **Aider Code Editing**: Code refactoring / editing pass rate.
- **Persistence**: `localStorage` automatic saving and state restoration on page load.

---

## 2. What's Left (Next Priorities)
- **Export / Share Feature**: Allow users to export or share their configured simulator settings.
- **Visual Charting**: Optional canvas-based breakdown showing proportion of context vs output vs thinking tokens per task.
- **Custom Plan Override**: Allow power users to input custom token ceilings.

---

## 3. Context & Gotchas
- **Zero-Build UI**: Pure HTML5/JS/Tailwind without a build step for portability.
