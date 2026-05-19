
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

---

## 2026-05-19 22:50 UTC — Viral retrofit: `ai-coding-assistant-cost-calc`

**Audit (pre-retrofit)** — 32 tools scanned; 5 already had all four mechanics (ai-cost-calculator, ai-disclosure-generator, github-roast, prompt-grade, what-ai-are-you); 27 missing.

**Tool picked**: `ai-coding-assistant-cost-calc` — AI-era (Cursor/Copilot/Claude Code search traffic), quantifiable result ($ savings for team-of-N), missing all four mechanics.

**Viral mechanics added:**
- [x] Share-on-X button — prefilled: "I priced N dev seats across 14 AI coding assistants — cheapest is X at $Y/mo. Annual swing vs worst pick: $Z. Compare yours →"
- [x] Copy-link button — copies deep-link encoding `seats|billing|usage|flags|filter` in URL hash
- [x] Embeddable shields.io badge — "AI coding cost: save $X/yr" with green/blue color tier
- [x] PNG download — 1200×630 canvas card with cheapest plan, annual swing highlight, brand bottom-right (tinytools-smoky.vercel.app)
- [x] Auto-load from URL hash + hashchange listener — deep-links reproduce the exact comparison

**Implementation notes (autonomous choices):**
- Hash format is compact (`10|monthly|moderate|000000|all`) so shared URLs stay short
- Embed badge color tiers: $5k+/yr=brightgreen, $1k+/yr=green, else=blue
- PNG card uses same dark gradient + cyan accent as the tool itself for brand consistency
- `history.replaceState` used so the user doesn't accumulate hash entries while tweaking inputs

**Verification:**
- Live raw fetch of `/ai-coding-assistant-cost-calc/index.html` confirms `twitter.com/intent/tweet` (1), `img.shields.io` (1), `location.hash` (3), `toDataURL` (1), `vmCardCanvas` (2)
- JS parses clean (`node --check`)
- Commit: `f4db8ac6fd50b537b33b27ff0689833d85e05871`

**Dashboard updated:** `dashboard/data.json` activity log + lastUpdated + visitorsDelta updated. Commit `e75339f62f48b982ac88bd70a5b7de77e986650a`.

**Counters:**
- Current visitor count (abacus tinytools-smoky/root): **1**
- Tools with all viral mechanics: **6** (was 5)
- Tools remaining without viral mechanics: **26**
