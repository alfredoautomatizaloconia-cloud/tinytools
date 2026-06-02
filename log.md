## 2026-06-01 — Viral Retrofit: background-remover

### Tool Retrofitted
- **background-remover** — 0 viral mechanics → full suite
  - URL: https://tinytools-smoky.vercel.app/background-remover/
  - Commit: f298f55d88ac

### Viral Mechanics Added
1. Share on X — prefills tweet "I removed the background from my image in-browser — free, no upload, no API key"
2. Copy-link — copies `#done` deep-link URL (images are local; hash signals shared result)
3. PNG download — 1200×630 canvas card with before/after checkerboard preview + brand footer
4. Embed badge — shields.io badge: `Background-Removed_Free-ec4899`
5. Hash deep-link — checks `location.hash === '#done'` on load, logs welcome message

### Stats
- Visitor count (abacus root): 1
- Tools audited: 45 (all dirs with index.html)
- Tools remaining without viral mechanics: 0 🎉 all tools now viral-ready

---

## 2026-06-01 — Viral Retrofit: domain-generator

### Tool Retrofitted
- **domain-generator** — 0 viral mechanics → full suite
  - URL: https://tinytools-smoky.vercel.app/domain-generator/
  - Commit: 9ca68a530f863ab1ca4e6ea7f2d89de6db8591c9

### Viral Mechanics Added
1. Share on X — prefills tweet with available domain count and deep-link
2. Copy-link — copies #keyword|style hash URL
3. PNG download — 1200x630 canvas card (keyword, count, brand footer)
4. Embed badge — shields.io badge with available domain count
5. Hash deep-link — auto-loads search from URL hash on page load

### Stats
- Visitor count (abacus root): 1
- Tools still missing viral mechanics: 3 (background-remover, chat-with-pdf, pdf-to-markdown)

---

## 2026-05-31 — ai-cofounder-match, devops-disaster-score

### Tools Shipped
- **ai-cofounder-match** (Tier 0 — Viral)
  - URL: https://tinytools-smoky.vercel.app/ai-cofounder-match/
  - HTTP: 200 ✅
  - Mechanic: 6-question quiz → AI cofounder match (ChatGPT / Claude / Gemini / Grok / Llama / Mistral)
  - Viral features: shareable PNG card, Share to X, deep-linkable hash, embeddable badge, deterministic scoring
  - Color: fuchsia #d946ef

- **devops-disaster-score** (Tier 0 — Viral)
  - URL: https://tinytools-smoky.vercel.app/devops-disaster-score/
  - HTTP: 200 ✅
  - Mechanic: paste GitHub repo URL → disaster score 0–100 from real GitHub API data
  - Viral features: shareable PNG card, Share to X, deep-linkable hash, embeddable badge, deterministic scoring
  - Color: red #dc2626

### Updates
- sitemap.xml: both added with priority 1.0
- index.html: both cards added with NEW·VIRAL badge at top of grid



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

---

## 2026-05-30 04:52 UTC — viral-retrofit: seo-meta-generator

**Task:** tinytools-viral-loop (scheduled, every 6h)
**Tool retrofitted:** seo-meta-generator
**Commit:** b6f00359ff0560f3c56637e3b4d125b97c23f350
**URL:** https://tinytools-smoky.vercel.app/seo-meta-generator/

**Viral mechanics added:**
- ✅ 𝕏 Share button — prefilled tweet with page title + char counts (title/60, desc/160)
- ✅ Copy deep link — full input state encoded as base64(JSON) in URL hash
- ✅ Embeddable shields.io badge — green=SEO Ready, orange=Needs Fix (based on char counts)
- ✅ 1200×630 PNG card download via canvas (title, domain, description, stats row, TinyTools brand)
- ✅ Auto-load from URL hash on page load (all 8 input fields restored from deep link)

**Current visitor count (abacus root):** 1
**Tools remaining without full viral mechanics:** 8
  (background-remover, color-palette, cover-letter-generator, domain-generator,
   mcp-server-inspector, pdf-to-markdown, resume-tailorer, youtube-to-blog)

**Selection rationale:** seo-meta-generator chosen over color-palette and cover-letter-generator
because SEO tools have high organic search traffic and the quantifiable results (char counts,
platform-ready status) make the share tweet feel earned and data-driven.

---

## 2026-05-30 — Scheduled Ship

**Tools shipped:** tweet-roaster, ai-pickup-lines
**Tier:** 0 (viral)
**Viral mechanics:** yes (both tools)

### tweet-roaster
- URL: https://tinytools-smoky.vercel.app/tweet-roaster/
- HTTP: 200 ✅
- Input: @handle + paste tweets textarea
- Analysis: 11 signals (hashtag density, buzzwords, self-promo ratio, humblebrags, thread addiction, emoji count, avg length, question ratio, link ratio, caps tweets, tweet count)
- Grade: F–S (10 tiers) with personality labels ("Thought Leader Cosplay", "Cringe Singularity", etc.)
- Viral mechanics: personal result ✅, canvas PNG card 1200×630 ✅, Share to X ✅, deep-linkable hash (handle|base64stats) ✅, shields.io badge ✅, reaction-bait copy ✅
- Color: sky #0ea5e9

### ai-pickup-lines
- URL: https://tinytools-smoky.vercel.app/ai-pickup-lines/
- HTTP: 200 ✅
- Input: name + AI tool dropdown (10 options)
- Pool: 70+ pickup lines across 10 categories (neural, programming, prompts, models, general, data, tool-specific)
- Charm score: deterministic 1–10 from name hash
- Personality archetypes: 10 types ("Legendary Charmer", "Chaotic Romantic", etc.)
- Regenerate button with variant seeds
- Viral mechanics: personal result ✅, canvas PNG card 1200×630 ✅, Share to X ✅, deep-linkable hash (name|tool) ✅, shields.io badge ✅, reaction-bait copy ✅
- Color: pink #ec4899

**Landing page:** updated, live count 39→41
**Sitemap:** both added at priority 1.0

**Tier 0 remaining (not yet shipped):** ai-cofounder-match, devops-disaster-score, saas-burn-roast

### viral-retrofit — 2026-05-30 22:51 UTC

**Tool retrofitted:** cover-letter-generator
**Commit:** de1cc95c717e1a7e2da2ea0bc8afed76b1d8aa09

**Viral mechanics added:**
- 🐦 Share on X — tweet prefilled: "Just generated an AI cover letter for \"[job title]\" in ~30 sec. Free, no signup, BYOK →"
- 🔗 Copy deep-link — encodes job title in URL hash
- 💾 Download card — 1200×630 canvas PNG with letter preview + TinyTools brand
- 🏷️ Embeddable badge — shields.io badge with job title slug
- 🔗 Auto-load from URL hash — #job-title pre-populates job field placeholder for deep-link visits

**Visitor count (tinytools-smoky/root):** 1
**Tools remaining without viral mechanics:** 8 (background-remover, c2pa-manifest-generator, chat-with-pdf, domain-generator, mcp-server-inspector, pdf-to-markdown, resume-tailorer, youtube-to-blog)
## 2026-05-31 04:51 UTC

**Tool retrofitted:** resume-tailorer  
**Viral mechanics added:**
- 𝕏 Share button — pre-filled tweet with job title + keyword count
- 🔗 Copy-link button — deep-link URL with job description encoded in hash
- 📛 Embeddable badge — shields.io ATS Optimized badge with keyword count
- 💾 PNG card download — 1200×630 canvas card via toDataURL
- Auto-load from URL hash — job description pre-fills on deep-link open

**Commit:** a5de569f3d15216267de46c40dbc1d64e2ef4f6b  
**Current visitor count (root):** 1  
**Tools remaining without viral mechanics:** ~7 (domain-generator, mcp-server-inspector, youtube-to-blog, background-remover, c2pa-manifest-generator, chat-with-pdf, pdf-to-markdown)

---## 2026-05-31 10:51 UTC

**Tool retrofitted:** mcp-server-inspector
**Viral mechanics added:**
- 𝕏 Share on X — tweet prefilled: "I just audited owner/repo with MCP Server Inspector: Grade X · Score Y/100 →"
- 🔗 Copy-link button — deep-link URL with repo encoded in URL hash (#owner/repo)
- 📛 Embeddable badge — shields.io badge with grade + score, colour-coded (green A → red F)
- 💾 PNG card download — 1200×630 canvas card via toDataURL with findings stats + TinyTools brand
- 🔗 Auto-load from URL hash — decodes hash and re-runs audit automatically for deep-link visits

**Commit:** e25a5867f665795c109b3d49baac2dd93e6e67ed
**Current visitor count (tinytools-smoky/root):** 1
**Tools remaining without viral mechanics:** 7 (domain-generator, background-remover, c2pa-manifest-generator, chat-with-pdf, pdf-to-markdown, youtube-to-blog, vs)

---

## 2026-05-31 — tinytools-viral-loop run

**Tool retrofitted:** youtube-to-blog  
**Viral mechanics added:**
- 𝕏 Share on X — tweet prefilled: "I just turned a YouTube video into an SEO blog post in seconds with AI ✍️"
- 🔗 Copy-link button — deep-link URL with video ID encoded in URL hash (#videoId)
- 📛 Embeddable badge — shields.io badge (Blog_Post-Generated, red YouTube-logo)
- 💾 PNG card download — 1200×630 canvas card via toDataURL with post title, excerpt, word count + TinyTools brand
- 🔗 Auto-load from URL hash — decodes #videoId and pre-fills the YouTube URL field on page load

**Commit:** 857572dc0ff5  
**Current visitor count (tinytools-smoky/root):** 1  
**Tools remaining without viral mechanics:** 5 (domain-generator, background-remover, c2pa-manifest-generator, chat-with-pdf, pdf-to-markdown)

---


## 2026-06-01 — Viral Retrofit: pdf-to-markdown

**Tool retrofitted:** `pdf-to-markdown`  
**Priority reason:** Quantifiable stats (pages/words/headings), developer audience, high Twitter engagement potential  

**Viral mechanics added:**
1. 🐦 **Share button** — prefills tweet with "Just converted a X-page PDF to Y words of clean Markdown 📄→✍️ No upload. 100% in-browser. Free. Try yours →" + deep-link
2. 🔗 **Copy-link button** — copies deep-link URL with encoded stats (format: `#Xp-Yw-Zh`)
3. 🏷 **Embeddable badge** — shields.io badge with real page/word counts, copy-on-click
4. 🖼 **PNG card download** — 1200×630 canvas card showing pages/words/headings/links stats with TinyTools brand, exported via `toDataURL`
5. 🔁 **Auto-load from URL hash** — detects `#Xp-Yw-Zh` on load, pre-populates meta strip and share panel so shared links feel alive

**Commit:** 6fd1392529ff5ec16aec1dc3f255c6b5ed508757  
**Current visitor count (tinytools-smoky/root):** 1  
**Tools remaining without viral mechanics:** 2 (background-remover, best-free-color-palette-generators-2026)

---
---

## 2026-06-02 — Daily Ship

### Tools Shipped

#### 1. startup-idea-roast (Tier 0 — Viral)
- **URL:** https://tinytools-smoky.vercel.app/startup-idea-roast/
- **HTTP:** 200 ✅
- **Concept:** Paste your startup idea, get a savage A–F roast + fake investor rejection letter + viability score
- **Viral mechanics:**
  1. ✅ Personal result — score/grade derived deterministically from idea text
  2. ✅ Shareable PNG card (1200×630 canvas with grade, roast snippet, score bar)
  3. ✅ Share to X button with pre-filled tweet including grade
  4. ✅ Deep-linkable URL (#encoded-idea reloads same result)
  5. ✅ Embeddable shields.io badge
  6. ✅ Reaction-bait copy ("brutal", "savage", "rejection letter")
- **Scoring:** deterministic rule engine — buzzword penalties, positive signal bonuses, length scoring; same input = same output

#### 2. ai-job-survival (Tier 0 — Viral)
- **URL:** https://tinytools-smoky.vercel.app/ai-job-survival/
- **HTTP:** 200 ✅
- **Concept:** Enter job title, get AI replacement probability, automation timeline, and survival tips
- **Viral mechanics:**
  1. ✅ Personal result — risk score from job title keyword/override database
  2. ✅ Shareable PNG card (1200×630 canvas with risk%, safety window, roast)
  3. ✅ Share to X button with pre-filled tweet
  4. ✅ Deep-linkable URL (#job-title reloads same result)
  5. ✅ Embeddable shields.io badge
  6. ✅ Reaction-bait copy ("The robots are coming", "your job", survival tips)
- **Scoring:** deterministic lookup table (60+ job overrides) + keyword matching; same input = same output

### Updates
- sitemap.xml updated (50 URLs total, both new tools at priority 1.0)
- index.html updated (tool count: 41 → 43, new cards at top of grid)

### Notes
- All TIER 0 tools from original roadmap are now shipped
- Inventing new viral tools extending the roadmap going forward

