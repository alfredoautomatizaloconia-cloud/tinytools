
## 2026-05-19 — Daily ship (viral mechanics)
- **what-ai-are-you** — Tier 0 viral. Buzzfeed-style 10-question personality quiz mapping users to one of 8 AI models (ChatGPT/Claude/Gemini/Grok/Llama/Perplexity/Mistral/DeepSeek). Deep-linkable via answer-index hash, shareable PNG card, X share, shields.io embed badge, JSON-LD schema. HTTP 200.
- **prompt-grade** — Tier 0 viral. Paste an AI prompt → deterministic A–F grade across 22 quality signals (role, task verb, context, format, examples, constraints, anti-hallucination, edge cases, audience, tone, length, CoT, delimiters, etc.) + savage one-line roast. Deep-linkable via base64 hash, shareable PNG card, X share, shields.io embed badge, JSON-LD schema. HTTP 200.

**Viral mechanics included (both tools):**
- [x] Personal result (per-user grade / per-user AI archetype)
- [x] Shareable PNG card (1200×630, canvas-rendered)
- [x] Share to X button with prefilled hook
- [x] Deep-linkable URL hash (same input → same result)
- [x] Embeddable shields.io badge
- [x] Reaction-bait copy ("savage", "your", "I got")
- [x] Single-file, pure browser, deterministic — no LLM cost

**URLs:**
- https://tinytools-smoky.vercel.app/what-ai-are-you/
- https://tinytools-smoky.vercel.app/prompt-grade/

Sitemap updated (priority 1.0 for both). Landing page features both tools with "NEW · VIRAL" badges. Tools-live counter → 37.
