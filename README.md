# LLM Quota & Model Comparison (Non-API Edition)

A standalone, interactive comparator and simulation engine built specifically for **account-based, non-API AI models and subscriptions** (Google Antigravity / AI Pro & Ultra, Anthropic Claude Pro & Max, and OpenAI ChatGPT Plus & Pro).

Unlike API calculators that meter costs by input/output tokens, this tool evaluates the real constraints that developers face in IDEs and web apps: **5-hour rolling token windows**, **weekly soft limits**, **agentic thinking overhead**, and **plan-tier multipliers ($20/mo vs $100/mo vs $200/mo)**.

---

## 🚀 Quick Start

### Option 1: Double-Click (macOS)
Double-click [`launch.command`](launch.command) in Finder to open the application directly in your default browser.

### Option 2: Terminal
```bash
open index.html
```

### Option 3: Local Web Server
```bash
python3 -m http.server 8000
# Open http://localhost:8000 in your browser
```

---

## ⚡ Features

- **20 Frontier Models Covered**:
  - **Google (Antigravity & AI Studio)**: Gemini 3.8 Flash (High/Low), Gemini 3.7 Flash (High/Low), Gemini 3.6 Flash (High/Low).
  - **Anthropic (Claude.ai & Claude Code)**: Claude Opus 5.5 (Standard & Adaptive Reasoning), Opus 5 (Standard & Extended Reasoning), Claude Sonnet 5 (Standard & Adaptive Reasoning), Claude Fable 5.1 (Standard & Deep Agentic Reasoning).
  - **OpenAI (ChatGPT Work & Codex)**: GPT-6 Sol (Standard & High Reasoning), GPT-6 Astra (Standard & Computer-Use Reasoning), GPT-6 Terra (Standard & Reasoning Mode).
- **Accurate 2026 Plan Tier Scaling**:
  - **Google**: Free, Google AI Plus ($4.99/mo), Google AI Pro ($19.99/mo), Google AI Ultra 5x ($100.00/mo), Google AI Ultra 20x ($200.00/mo), Antigravity Enterprise ($35.00/mo).
  - **Anthropic**: Claude Free, Claude Pro ($20.00/mo), Claude Team ($30.00/user/mo), Claude Max 5x ($100.00/mo), Claude Max 20x ($200.00/mo).
  - **OpenAI**: ChatGPT Free, ChatGPT Plus ($20.00/mo), ChatGPT Business ($30.00/user/mo), ChatGPT Pro 5x ($100.00/mo), ChatGPT Pro 20x ($200.00/mo).
- **Interactive 5-Hour Workload Simulator**:
  - Sliders for turn count and context payload.
  - Dynamically calculates token consumption (including hidden reasoning tokens) and warns before triggering rolling window lockouts.
- **Head-to-Head 3-Way Comparison**:
  - Select any 3 models to compare plan costs, rolling budgets, context ceilings, and reset policies side-by-side.
- **Offline & Local Storage Persistence**:
  - All selections (plans, models, simulator sliders) are auto-saved to your browser's `localStorage` so your configuration is remembered on reload.
  - 100% self-contained single-file HTML application.

---

## 📖 In-Depth Guide

For complete technical documentation on rate limit reset cycles, banked resets, and strategies to prevent cooldowns in coding agents, see [`GUIDE.md`](GUIDE.md).

---

## 📄 License

MIT License. See [`LICENSE`](LICENSE) for details.
