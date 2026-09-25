# Project Status & Handoff Tracking (`PROGRESS.md`)

## 1. Where We Stand
- **Core System**: Self-contained client-side web application (`index.html`) implementing the Non-API Model & Quota Comparator.
- **Model Coverage**: 22 model variations across Google (Gemini 3.8/3.7/3.6 Flash High & Low, Gemini 3.1 Pro High & Low), Anthropic (Claude Opus 5.5, Opus 5, Sonnet 5, Fable 5.1 Standard & Reasoning), and OpenAI (GPT-6 Sol, Astra, Terra Standard & Reasoning).
- **Accurate 2026 Limits**: 
  - Verified and updated Claude Opus 5.5, Sonnet 5, and Fable 5.1 to 1,000,000 token context window and 128k output.
  - Verified and updated GPT-6 Sol, Astra, and Terra to 1,050,000 token context window and 128k output.
- **Subscription Multipliers**: Accurate live 2026 pricing and quota multipliers for:
  - Google: Free ($0), Plus ($4.99), Pro ($19.99), Ultra 5x ($100), Ultra 20x ($200), Enterprise ($35).
  - Anthropic: Free ($0), Pro ($20), Team ($30), Max 5x ($100), Max 20x ($200).
  - OpenAI: Free ($0), Plus ($20), Business ($30), Pro 5x ($100), Pro 20x ($200).
- **Persistence**: `localStorage` automatic saving and state restoration on page load.
- **Launchers**: macOS `launch.command` verified executable.
- **Documentation**: Comprehensive `GUIDE.md` and `README.md` included.

---

## 2. What's Left (Next Priorities)
- **Export / Share Feature**: Allow users to export or share their configured simulator settings via URL query parameters or JSON snippets.
- **Visual Charting**: Optional canvas-based breakdown showing proportion of context vs output vs thinking tokens per task.
- **Custom Plan Override**: Allow power users to input custom token ceilings if their enterprise contract has specialized quotas.

---

## 3. Context & Gotchas
- **Reasoning Token Mechanics**: Thinking tokens in Gemini 3.8/3.7 Flash and Claude Opus 5.5 count toward the output and 5-hour rolling pool limits. In the simulator, reasoning modes apply a `1.45x` to `1.75x` token multiplier to simulate this hidden consumption.
- **No Build Step Required**: The application deliberately uses a zero-build architecture (pure HTML5 + JavaScript + Tailwind via safe CDN with CSS variable fallbacks). It requires no Node.js or bundling step to maintain maximum portability.
