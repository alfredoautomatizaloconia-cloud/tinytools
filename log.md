
## 2026-05-21 — Daily Ship

### Tool 1: ai-text-roast
- **Tier**: 0 (Viral)
- **URL**: https://tinytools-smoky.vercel.app/ai-text-roast/
- **HTTP**: 200 ✅
- **Viral mechanics**: ✅ Personal AI % score · ✅ Shareable 1200×630 PNG card · ✅ X share button prefilled · ✅ Deep-linkable URL hash · ✅ Embeddable shields.io badge
- **Engine**: Deterministic heuristic (AI phrase dict, lexical diversity, burstiness, sentence variance) — no API, fully browser-side

### Tool 2: roast-my-resume
- **Tier**: 0 (Viral)
- **URL**: https://tinytools-smoky.vercel.app/roast-my-resume/
- **HTTP**: 200 ✅
- **Viral mechanics**: ✅ Letter grade A+–F · ✅ Shareable 1200×630 PNG card · ✅ X share prefilled with grade · ✅ Deep-linkable URL hash · ✅ Embeddable shields.io badge
- **Engine**: 5-dimension deterministic scorer (Impact, Action Verbs, Buzzword Toxicity, Structure, Differentiation) — no API, fully browser-side


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

---

## 2026-05-21 — Viral Retrofit Run

**Tool retrofitted:** `mcp-config-generator`

**Why chosen:** Highest-priority AI-era tool. MCP (Model Context Protocol) is the hottest developer topic in 2026. Targets developers with high share intent. Was missing all 4 viral markers.

**Viral mechanics added:**
- ✅ **𝕏 Share button** — prefills tweet with server count, stack names, deep-link URL
- ✅ **Copy-link button** — copies deep-link with host + server IDs in hash (`#claude-desktop:filesystem,github,slack`)
- ✅ **Embeddable badge** — shields.io badge showing MCP stack size, copyable HTML for READMEs
- ✅ **PNG card download** — 1200×630 canvas card with server chips, host, count, TinyTools branding
- ✅ **Hash auto-load** — deep-links fully restore state (host + checked servers)

**Commit:** `74dfa1d4cfcc0ff945b973a6b809b29fbe888d0e`

**Current visitor count (root):** 1
**Tools with viral mechanics now:** 11 / 26 audited
**Tools still missing viral mechanics:** 15
- ai-prompt-enhancer, ai-robots-txt-generator, eu-ai-act-risk-assessment, color-palette, favicon-generator, og-image-generator, cover-letter-generator, resume-tailorer, seo-meta-generator, domain-generator, llm-prompt-optimizer, voice-cloning-detector, c2pa-manifest-generator, youtube-to-blog, prompt-injection-tester
