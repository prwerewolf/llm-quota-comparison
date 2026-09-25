# Changelog

All notable changes to this project will be documented in this file.

## [1.0.0] - 2026-09-25

### Added
- Initial release of the Non-API Model & Quota Comparator.
- Interactive plan selectors for Google (Free, Plus, Pro, Ultra 5x, Ultra 20x, Enterprise), Anthropic (Free, Pro, Team, Max 5x, Max 20x, Enterprise), and OpenAI (Free, Plus, Business, Pro 5x, Pro 20x, Enterprise).
- Full specifications and non-API quota metrics for 20 frontier models (Gemini 3.8/3.7/3.6 Flash, Claude Opus 5.5, Opus 5, Sonnet 5, Fable 5.1, GPT-6 Sol, Astra, Terra).
- Plan-aware 5-Hour Workload Simulator with token consumption estimation and lockout alerts.
- Head-to-Head 3-slot comparative matrix.
- `localStorage` automatic state persistence.
- Double-clickable macOS `launch.command` script.
- In-depth non-API comparative guide (`GUIDE.md`).

## [1.1.0] - 2026-09-25

### Added
- Added Gemini 3.1 Pro (High and Low) to the comparator.

### Fixed
- Corrected late 2026 model limits based on live data (Opus 5.5, Sonnet 5, Fable 5.1 context updated to 1M with 128k output).
- Corrected GPT-6 models (Sol, Astra, Terra) context updated to 1.05M with 128k output.

## [1.2.0] - 2026-09-25

### Added
- Vibe Coding Evaluation Scores integrated into model comparison.
- Models now display SWE-bench Verified (Agentic Autonomy), Chatbot Arena Coding Elo (Human Preference), and Aider Code Editing (Refactor Pass Rate).
- Dedicated "Vibe Coding Industry Evals" UI component in the model inspector.
- Head-to-Head Compare view and Master Ledger table now include eval metrics.

## [1.3.0] - 2026-09-25

### Added
- Integrated Instruction Following (IFEval), Context Recall (NIAH), and LiveCodeBench scores into the model comparator.
- Added explanatory hover tooltips (using native `title` and CSS dashed underlines) to all 6 Vibe Coding evaluation metrics in the Inspector and Compare views.

## [1.4.0] - 2026-09-25

### Added
- Added "🏆 BEST" dynamic highlighting to the Head-to-Head Compare table. The view now automatically calculates and highlights the top-scoring model for each of the 6 Vibe Coding evaluation metrics, dimming the losing scores to make comparisons instantly readable.
