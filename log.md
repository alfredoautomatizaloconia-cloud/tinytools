

---

## 2026-05-29 — Daily Ship Run

**Tools shipped:** roast-my-landing-page, ai-spend-calculator
**Tier:** 0 (viral)

### Tool 1: roast-my-landing-page
- **URL:** https://tinytools-smoky.vercel.app/roast-my-landing-page/
- **HTTP:** 200 ✅
- **Concept:** Paste a URL → AI fetches the page via CORS proxy and grades 14 conversion signals (CTAs, social proof, mobile viewport, meta tags, pricing, FAQ, demos, script count, word density) → A–F grade + savage roast
- **Accent color:** #f97316 (orange)
- **Viral mechanics:**
  - ✅ Personal result (URL-specific grade about YOUR page)
  - ✅ Shareable 1200×630 PNG canvas card with URL embedded
  - ✅ Share to X with pre-filled tweet including grade + roast
  - ✅ Deep-linkable URL (hash = base64 encoded input URL)
  - ✅ Embeddable shields.io badge (Landing_Page_Grade)
  - ✅ Loading step-by-step animation (fetching → parsing → grading → roasting)
  - ✅ Signal breakdown list (6 detailed signals per page)
  - ✅ JSON-LD WebApplication schema
  - ✅ Long-form SEO section

### Tool 2: ai-spend-calculator
- **URL:** https://tinytools-smoky.vercel.app/ai-spend-calculator/
- **HTTP:** 200 ✅
- **Concept:** Check every AI tool you subscribe to (17 tools with tier pricing) + API spend → yearly total + percentile rank + archetype label (Free Rider / Dabbler / Power User / AI Addict / AI Baller / AI Maximalist) + savage roast
- **Accent color:** #10b981 (green)
- **Tools covered:** ChatGPT, Claude, Gemini, Grok, Perplexity, Cursor, Copilot, Windsurf, Devin, Midjourney, Runway, Sora, ElevenLabs, Notion AI, Grammarly, Canva Pro, Otter.ai + OpenAI/Anthropic/Other API
- **Viral mechanics:**
  - ✅ Personal result (your spend, your rank, your archetype)
  - ✅ Shareable 1200×630 PNG canvas card
  - ✅ Share to X with pre-filled tweet including $amount + percentile
  - ✅ Deep-linkable URL (hash = base64 JSON of selected tools + tiers + API amounts)
  - ✅ Embeddable shields.io badge (AI_Spender archetype + yearly amount)
  - ✅ Breakdown bar chart of spend per tool
  - ✅ 6 dynamic achievement badges
  - ✅ JSON-LD WebApplication schema
  - ✅ Long-form SEO section

**Sitemap:** Both added with priority 1.0, changefreq weekly
**Landing page:** Both cards added to index.html in viral tools section (top)

---

## 2026-05-29 — vs/claude-pro-pricing comparison page

**Task:** tinytools-comparison-pages (scheduled)
**Page:** https://tinytools-smoky.vercel.app/vs/claude-pro-pricing/
**Competitor:** Claude Pro ($20/month — Anthropic AI assistant)
**HTTP status:** 200 ✅
**Total /vs/ pages:** 45
**Sitemap:** Added at priority 0.7, changefreq monthly
**Notes:** First unshipped competitor from rotation list (items 1–18 already shipped). Page covers LLM pricing comparison angle with internal links to llm-prompt-optimizer, ai-spend-calculator, ai-cost-calculator, ai-text-detector, prompt-grade, ai-prompt-enhancer, and prompt-injection-tester.
