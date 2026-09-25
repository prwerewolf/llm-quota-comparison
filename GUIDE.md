# Non-API Model & Quota Comparative Guide (Multi-Plan Edition)

> [!NOTE]
> This guide is calibrated for **non-API, account-based subscriptions**. In non-API environments (Antigravity, Claude Code, ChatGPT Work/Codex), your account subscription tier directly governs your **5-hour rolling session budget**, **weekly fair-use cap**, and **cooldown/lockout policies**.

---

## 1. Provider Subscription Plan Tiers & Scaling Ratios (September 2026)

The AI subscription landscape across Google, Anthropic, and OpenAI has structured itself into aligned pricing tiers: **\$20/mo (Standard Individual)**, **\$100/mo (Power User / 5x)**, and **\$200/mo (Top Frontier / 20x)**.

### A. Anthropic Claude Subscriptions
* **Claude Free (\$0/mo)**:
  - Multiplier: `~0.15x`.
  - Quota: ~10–15 messages every 5 hours. Flagship models (Opus 5.5, Fable 5.1) are locked or restricted to minimal trial turns; daily driver is Sonnet fallback. Does not include Claude Code.
* **Claude Pro (\$20.00/mo)**:
  - Multiplier: `1.0x` (Baseline Individual).
  - Quota: ~450,000 tokens per 5h on Opus 5.5 Standard (~55 msgs); ~280,000 tokens on Adaptive Reasoning (~30 turns); ~900,000 tokens on Sonnet 5 (~100 msgs).
  - Includes **1 Banked Rate-Limit Reset** and access to Claude Code & Claude Cowork.
* **Claude Team (\$25–\$30/user/mo)**:
  - Multiplier: `1.4x`.
  - Quota: ~630,000 tokens per 5h on Opus 5.5 Standard (~75 msgs); ~390,000 tokens on Adaptive Reasoning (~42 turns). Includes team administration and shared billing.
* **Claude Max 5x (\$100.00/mo)**:
  - Multiplier: `5.0x`.
  - Quota: ~2,250,000 tokens per 5h on Opus 5.5 Standard (~250+ msgs); ~1,400,000 tokens on Adaptive Reasoning (~140 turns).
  - Extended context window enabled up to **500,000 tokens**; includes **2 Banked Rate-Limit Resets**.
* **Claude Max 20x (\$200.00/mo - Top Power User Tier)**:
  - Multiplier: `20.0x`.
  - Quota: **~9,000,000 tokens** per 5h on Opus 5.5 Standard (~1,000+ msgs); **~5,600,000 tokens** on Adaptive Reasoning (~550+ deep turns); **~18,000,000 tokens** on Sonnet 5.
  - Built specifically for all-day intensive agentic coding, repository-scale rewrites in Claude Code, and deep multi-hour research workflows without cooldown interruptions.
* **Claude Enterprise (\$Custom)**:
  - Dedicated capacity, highest priority during peak traffic, enterprise SSO, and HIPAA compliance options.

---

### B. Google AI Subscriptions (Antigravity & AI Studio)
* **Google AI Free (\$0/mo)**:
  - Multiplier: `~0.25x` baseline.
  - Quota: 5-hour rolling pool capped at ~350,000 tokens for Flash High. Weekly refresh with strict throttles once reached.
* **Google AI Plus (\$4.99/mo)**:
  - Multiplier: `~0.5x`.
  - Quota: 2x Free limits with 400 GB cloud storage.
* **Google AI Pro (\$19.99/mo)**:
  - Multiplier: `1.0x` (Everyday Pro Tier).
  - Quota: ~1.4M tokens per 5h window on Gemini 3.8 Flash High; ~3.5M on Flash Low. Full 1,048,576 context window. Includes 5 TB storage.
* **Google AI Ultra 5x (\$100.00/mo)**:
  - Multiplier: `5.0x`.
  - Quota: ~7.0M tokens per 5h window on 3.8 Flash High (~125 turns); ~17.5M on Flash Low. Priority queueing for Antigravity, Deep Think access, and 20 TB cloud storage.
* **Google AI Ultra 20x (\$200.00/mo - Top VIP Tier)**:
  - Multiplier: `20.0x`.
  - Quota: **~28,000,000 tokens** per 5h on Gemini 3.8 Flash High (~500+ deep turns); **~70,000,000 tokens** on Flash Low. Includes Project Genie, Gemini Spark, 30 TB storage, and dedicated Antigravity hardware prioritization.
* **Antigravity Enterprise / Workspace (\$35.00/user/mo)**:
  - Multiplier: `3.5x`.
  - Quota: Pooled team quota (~4.9M tokens / 5h per active seat) with background AI credit overage fallback for continuous agent orchestration.

---

### C. OpenAI ChatGPT Subscriptions
* **ChatGPT Free (\$0/mo)**:
  - Multiplier: `~0.1x`.
  - Quota: GPT-6 Sol restricted to a few introductory turns/day; Astra is unavailable; Terra operates under strict rate limits.
* **ChatGPT Plus (\$20.00/mo)**:
  - Multiplier: `1.0x` (Baseline Individual).
  - Quota: ~1.2M tokens per 5h on GPT-6 Sol Standard (~95 msgs); ~650,000 tokens on High Reasoning (~40 msgs); ~500,000 tokens on GPT-6 Astra Standard (~40 msgs); ~350,000 tokens on Astra Agentic Reasoning (~20 msgs).
* **ChatGPT Business (\$25–\$30/user/mo)**:
  - Multiplier: `1.8x`.
  - Quota: ~2.1M tokens per 5h on Sol Standard (~170 msgs); ~900,000 tokens on Astra Standard (~70 msgs). Shared team workspace and administrative controls.
* **ChatGPT Pro 5x (\$100.00/mo)**:
  - Multiplier: `5.0x`.
  - Quota: 5x Plus limits across models with dedicated compute during peak hours.
* **ChatGPT Pro 20x (\$200.00/mo - Frontier Tier)**:
  - Multiplier: `20.0x` (or **Virtually Uncapped** on Sol & Terra).
  - Quota: Sol and Terra are unthrottled under normal coding agent usage. Astra 5-hour limit scaled 20x to **~7,000,000+ tokens** (~400+ agent turns) with unthrottled computer-use compute.
* **ChatGPT Enterprise (\$Custom)**:
  - Unlimited high-speed frontier access, maximum context window retention, and audit logs.

---

## 2. Comparative Matrix Across All Key Plan Tiers

The table below shows effective 5-hour rolling allowances across **Standard (\$20/mo)**, **Mid Power (\$100/mo)**, and **Top Power (\$200/mo)** plans:

| Model Variation | Standard / Pro / Plus (\$20/mo) | Power Tier (\$100/mo - 5x) | Top Frontier Tier (\$200/mo - 20x) |
| :--- | :--- | :--- | :--- |
| **Gemini 3.1 Pro (High)** | ~1.8M tok (~40 turns) [AI Pro] | ~9.0M tok (~200 turns) [Ultra $100] | **~36.0M tok (~800 turns)** [Ultra $200] |
| **Gemini 3.1 Pro (Low)** | ~4.5M tok (~100 turns) [AI Pro] | ~22.5M tok (~500 turns) [Ultra $100] | **~90.0M tok (~2,000 turns)** [Ultra $200] |
| **Gemini 3.8 Flash (High)** | ~1.4M tok (~25 turns) [AI Pro] | ~7.0M tok (~125 turns) [Ultra \$100] | **~28.0M tok (~500 turns)** [Ultra \$200] |
| **Gemini 3.8 Flash (Low)** | ~3.5M tok (~85 turns) [AI Pro] | ~17.5M tok (~425 turns) [Ultra \$100] | **~70.0M tok (~1,700 turns)** [Ultra \$200] |
| **Gemini 3.7 Flash (High)** | ~1.6M tok (~35 turns) [AI Pro] | ~8.0M tok (~175 turns) [Ultra \$100] | **~32.0M tok (~700 turns)** [Ultra \$200] |
| **Gemini 3.7 Flash (Low)** | ~4.2M tok (~110 turns) [AI Pro] | ~21.0M tok (~550 turns) [Ultra \$100] | **~84.0M tok (~2,200 turns)** [Ultra \$200] |
| **Gemini 3.6 Flash (High)** | ~2.2M tok (~50 turns) [AI Pro] | ~11.0M tok (~250 turns) [Ultra \$100] | **~44.0M tok (~1,000 turns)** [Ultra \$200] |
| **Gemini 3.6 Flash (Low)** | ~5.5M tok (~150 turns) [AI Pro] | ~27.5M tok (~750 turns) [Ultra \$100] | **~110.0M tok (~3,000 turns)** [Ultra \$200] |
| **Claude Opus 5.5 (Standard)** | ~450k tok (~55 msgs) [Pro] | ~2.25M tok (~250+ msgs) [Max \$100] | **~9.0M tok (~1,000+ msgs)** [Max \$200] |
| **Claude Opus 5.5 (Reasoning)**| ~280k tok (~30 turns) [Pro] | ~1.40M tok (~140 turns) [Max \$100] | **~5.6M tok (~550 turns)** [Max \$200] |
| **Claude Opus 5 (Standard)** | ~250k tok (~40 msgs) [Pro] | ~1.25M tok (~180 msgs) [Max \$100] | **~5.0M tok (~750 msgs)** [Max \$200] |
| **Claude Opus 5 (Reasoning)** | ~180k tok (~20 msgs) [Pro] | ~900k tok (~95 turns) [Max \$100] | **~3.6M tok (~380 turns)** [Max \$200] |
| **Claude Sonnet 5 (Standard)** | ~900k tok (~100 msgs) [Pro] | ~4.50M tok (~500 msgs) [Max \$100] | **~18.0M tok (~2,000 msgs)** [Max \$200] |
| **Claude Sonnet 5 (Reasoning)**| ~550k tok (~50 msgs) [Pro] | ~2.75M tok (~240 turns) [Max \$100] | **~11.0M tok (~1,000 turns)** [Max \$200] |
| **Claude Fable 5.1 (Standard)** | ~320k tok (~35 turns) [Pro] | ~1.60M tok (~175 turns) [Max \$100] | **~6.4M tok (~700 turns)** [Max \$200] |
| **Claude Fable 5.1 (Reasoning)**| ~200k tok (~18 turns) [Pro] | ~1.00M tok (~90 turns) [Max \$100] | **~4.0M tok (~360 turns)** [Max \$200] |
| **GPT-6 Sol (Standard)** | ~1.2M tok (~95 msgs) [Plus] | ~6.0M tok (~450 msgs) [Pro \$100] | **Virtually Uncapped** [Pro \$200] |
| **GPT-6 Sol (Reasoning)** | ~650k tok (~40 msgs) [Plus] | ~3.25M tok (~200 msgs) [Pro \$100] | **~13.0M tok (~800 turns)** [Pro \$200] |
| **GPT-6 Astra (Standard)** | ~500k tok (~40 msgs) [Plus] | ~2.50M tok (~200 msgs) [Pro \$100] | **~10.0M tok (~800 msgs)** [Pro \$200] |
| **GPT-6 Astra (Reasoning)** | ~350k tok (~20 msgs) [Plus] | ~1.75M tok (~100 turns) [Pro \$100] | **~7.0M tok (~400 turns)** [Pro \$200] |
| **GPT-6 Terra (Standard)** | ~800k tok (~75 msgs) [Plus] | ~4.0M tok (~375 msgs) [Pro \$100] | **Virtually Uncapped** [Pro \$200] |
| **GPT-6 Terra (Reasoning)** | ~450k tok (~35 msgs) [Plus] | ~2.25M tok (~175 msgs) [Pro \$100] | **~9.0M tok (~700 turns)** [Pro \$200] |

---

## 3. How to Use the Interactive Comparator

Open [non_api_model_comparator.html](file:///Users/gregoryortiz/.gemini/antigravity/brain/748997bb-87cb-4003-a624-73f352888a8b/non_api_model_comparator.html):
1. **Directly Select Your Plan**:
   - Anthropic: Click **Claude Max 20x (\$200.00/mo)** to reflect your active subscription.
   - Google: Choose **Google AI Pro (\$19.99)** or **Google AI Ultra 20x (\$200.00)**.
   - OpenAI: Choose **ChatGPT Plus (\$20)** or **ChatGPT Pro 20x (\$200)**.
2. **Preset Button**:
   - Click the top purple button: **`★ Top $200/mo Tier (Max 20x / Ultra $200 / Pro $200)`** to align all providers to the \$200/mo flagship rate limits with a single click.
3. **Workload Simulator**:
   - Test heavy agentic tasks against your 20x allowance to observe how your \$200/mo plan eliminates cooldowns during day-long coding marathons.
