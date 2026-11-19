# REBUILD.md

> Auto-generated rebuild brief for **https://mattis.framer.website** (captured 2026-06-17T10:22:56.204Z)

## What you're rebuilding

- **Source**: https://mattis.framer.website
- **Page title**: Mattis® Studio — Conversion-First Design & Development Agency
- **Detected stack**: framer-motion, framer.com (built site), webflow, lenis
- **Recommended stack**: Next.js (App Router) + TypeScript + Tailwind CSS + Motion (framer-motion) + Lenis
- **Sections**: 11
- **Animations captured**: 1529
- **Assets**: 34

## Reference folder layout

```
reference/mattis/
├── meta.json                  # this capture's metadata
├── REBUILD.md                 # ← you are here
├── dom/full.html              # complete inlined dom
├── dom/sections/*.html        # per-section subtrees
├── screenshots/{desktop,tablet,mobile}-full.png
├── screenshots/sections/      # per-section, per-viewport
├── motion/animations.json     # raw capture
├── motion/motion-specs.md     # ★ READ THIS — durations + easings
├── assets/{images,videos,fonts}/  # everything harvested (hash-prefixed names)
├── assets/manifest.json       # original urls -> on-disk local paths
├── tokens/{colors,typography,spacing}.json
├── tokens/tokens.css          # ready-to-import css vars
├── tokens/fonts.css           # @font-face for captured fonts
└── stack/detected.md          # framework detection notes
```

## Rules of engagement (95%+ fidelity required)

This is a **1:1 reproduction**, not a "spiritually similar" rebuild. Concrete rules:

1. **Use the actual text.** Every headline, paragraph, button label, link is in `content/text.md` and `content/sections.json`. Do not paraphrase, do not "improve" copy, do not make up filler.
2. **Use the actual images.** Each section block below lists the **exact on-disk path** for every image (hash-prefixed, with the real detected extension — e.g. `assets/images/930cdbce-name.avif`). Copy those files into your project's `public/` and reference them. The bare original filenames do NOT exist on disk; use the paths as written, or `assets/manifest.json` (`originalUrl` → `localPath`) to resolve. If a section has a hero image, your section MUST have that exact image — not a CSS gradient stand-in.
3. **Use the actual fonts.** `tokens/fonts.css` has `@font-face` declarations for every captured woff2/ttf. Import it. Don't substitute Google Fonts unless the source font wasn't captured.
4. **For motion: EXACT values from `motion/motion-specs.md`.** No "ease-out", no "0.5s". Use the bezier arrays and durations as captured.
5. **For tokens: import `tokens/tokens.css`.** Don't pick new colors, font sizes, or spacing values.
6. **Build section-by-section.** Don't move on until your section matches the reference at all 3 viewports. Screenshot diff after each.
7. **Use the layout tree.** `content/layouts.json` has the structural skeleton — flex/grid directions, gaps, child order. Match it.
8. **Smooth scroll**: the source uses Lenis — install `lenis` and wire it up at the root.
9. **No placeholder content.** No "Lorem ipsum", no "Project Name", no fake stats. The real numbers, names, and copy are extracted.

## Sections — exact content (build verbatim)

> Every section below has its **exact text, images, fonts, and computed styles** captured. Do not rewrite copy. Do not pick new assets. Do not invent font sizes. Use what's here.


### 1. `01-hero`
*framer name: Hero*
**Background:** `rgb(255, 255, 255)`

- screenshot (desktop): `screenshots/sections/01-hero-desktop.png`
- screenshot (tablet): `screenshots/sections/01-hero-tablet.png`
- screenshot (mobile): `screenshots/sections/01-hero-mobile.png`
- dom subtree: `dom/sections/01-hero.html`
- structural layout tree: `content/layouts.json` → find `"slug": "01-hero"`

**Motion (204 animated · 0 fired during scroll):**
- defaults: 200ms × `ease`

**Scroll-linked motion (12 elements):**
- `Closed` `pinned` over scrollY 0→13207px
- `Navigation Menu` `pinned` over scrollY 0→13207px
- `Desktop` `pinned` over scrollY 0→13207px
- `Closed` `pinned` over scrollY 0→13207px
- `Bg blur` `pinned` over scrollY 0→13207px
- `BG blur` `pinned` over scrollY 0→13207px
- `Phone` `pinned` over scrollY 0→13207px
- `div` `pinned` over scrollY 0→13207px
- ...and 4 more (see `motion/scroll-motion.json`)
- **labels (small/uppercase):** `We` · `align` · `strategy,` · `design,` · `and` · `engineering` · `into` · `single` · `high-performance loop` · `high-performance` · `loop` · `Your` · `vision,` · `executed` · `with` · `surgical` · `precision` · `conversion-first` · `logic.` · `SLOTS FOR`

**Paragraphs:**
- "(Est. 2019 — Version 1.0.4)" — 11px / rgb(255, 255, 255)
- "Mattis" — 140.498px / rgb(255, 255, 255)
- "studio" — 34px / rgb(255, 255, 255)
- "We align strategy, design, and engineering into a single high-performance loop. Your vision, executed with surgical precision and conversion-first logic." — 12px / rgb(255, 255, 255)
- "Anna Schneider" — 13px / rgb(255, 255, 255)
- "CEO" — 11px / rgba(255, 255, 255, 0.6)
- "design" — 16px / rgb(255, 255, 255)
- "development" — 16px / rgb(255, 255, 255)

**Images (1):**
- small, 40×40 → `assets/images/58fe4b14-dvRbwMeyo4vxcTj90QvjS6MdQ.avif`

**Videos:**
- 375×710 → `assets/videos/91bd8e31-YUc1UMqfu6cFqEbpKpI1dpKqoes.mp4`

**CSS background-image urls:**
- on `div.`: `assets/images/1dae10b6-rR6HYXBrMmX4cRpXfXUOvpvpB0.png`

**Inline SVGs:** 2 (full markup in `content/sections.json`)

### 2. `02-about`
*framer name: About*
**Background:** `rgb(255, 69, 0)`

- screenshot (desktop): `screenshots/sections/02-about-desktop.png`
- screenshot (tablet): `screenshots/sections/02-about-tablet.png`
- screenshot (mobile): `screenshots/sections/02-about-mobile.png`
- dom subtree: `dom/sections/02-about.html`
- structural layout tree: `content/layouts.json` → find `"slug": "02-about"`

**Motion (307 animated · 3 fired during scroll):**
- defaults: 600ms × `ease`
- stagger group: 3 items, 80ms step, 600ms each, easing `cubic-bezier(0.68, 0, 0, 1)`
- 1 hover state(s): opacity (timing typically 0s ease)

**Scroll-linked motion (2 elements):**
- `Media` `parallax` over scrollY 0→4939px
- `Image` `parallax` over scrollY 0→4939px
- parallax: bind translateY to scrollYProgress with negative multiplier (e.g. `useTransform(p, [0,1], ['0%','-30%'])`)

**Hover states (1):**
- `svg:nth-child(3)` — changes: opacity — 0s `ease`
- **labels (small/uppercase):** `if they trust your site` · `spacing, typography, image quality, and structure`

**Headings:**
- h1: "Strategybeforepixels." — 52px / 600 / rgb(255, 255, 255) / family: `Geist`

**Paragraphs:**
- "Launched" — 12px / rgb(255, 255, 255)
- "24+ projects" — 12px / rgb(255, 255, 255)
- "2019-26©" — 12px / rgb(255, 255, 255)
- "People decide if they trust your site before they read a word on it. That's not a metaphor. Visual credibility forms almost instantly, and it's shaped by spacing, typography, image quality, and structure." — 12px / rgba(255, 255, 255, 0.7)
- "About us" — 13px / rgb(255, 255, 255)
- "About us" — 13px / rgb(255, 255, 255)
- "Industries where our sites consistently outperform benchmarks" — 13px / rgb(255, 255, 255)

**Links:** `About usAbout us`

**CSS background-image urls:**
- on `div.`: `assets/images/a2ee9050-eFCg3n7XxnLCImN4MelOsAGvIUY.avif`
- on `div.`: `assets/images/1dae10b6-rR6HYXBrMmX4cRpXfXUOvpvpB0.png`

**Inline SVGs:** 1 (full markup in `content/sections.json`)

### 3. `03-showreel`
*framer name: Showreel*
**Background:** `rgb(233, 233, 233)`

- screenshot (desktop): `screenshots/sections/03-showreel-desktop.png`
- screenshot (tablet): `screenshots/sections/03-showreel-tablet.png`
- screenshot (mobile): `screenshots/sections/03-showreel-mobile.png`
- dom subtree: `dom/sections/03-showreel.html`
- structural layout tree: `content/layouts.json` → find `"slug": "03-showreel"`

**Motion (61 animated · 3 fired during scroll):**
- defaults: 500ms × `ease`
- stagger group: 3 items, 60ms step, 500ms each, easing `cubic-bezier(0.68, 0, 0, 1)`

**Scroll-linked motion (1 elements):**
- `Media` `parallax` over scrollY 0→5780px
- parallax: bind translateY to scrollYProgress with negative multiplier (e.g. `useTransform(p, [0,1], ['0%','-30%'])`)
- **labels (small/uppercase):** `where moving forward feels` · `, and`

**Headings:**
- h2: "Webuildwebsites." — 52px / 600 / rgb(11, 11, 11) / family: `Geist`

**Paragraphs:**
- "2019-26©" — 12px / rgba(11, 11, 11, 0.6)
- "where moving forward feels obvious, natural, and impossible to overthink." — 12px / rgb(11, 11, 11)
- "↓ SEE THE WORK" — 12px / rgba(11, 11, 11, 0.6)
- "Showreel" — 12px / rgb(11, 11, 11)

**CSS background-image urls:**
- on `div.`: `assets/images/0b2d0529-ROGfhegDuACLsAjwXl6Yy1kaYzM.avif`

**Inline SVGs:** 1 (full markup in `content/sections.json`)

### 4. `04-works`
*framer name: Works*
**Background:** `rgb(233, 233, 233)`

- screenshot (desktop): `screenshots/sections/04-works-desktop.png`
- screenshot (tablet): `screenshots/sections/04-works-tablet.png`
- screenshot (mobile): `screenshots/sections/04-works-mobile.png`
- dom subtree: `dom/sections/04-works.html`
- structural layout tree: `content/layouts.json` → find `"slug": "04-works"`

**Motion (141 animated · 0 fired during scroll):**

**Scroll-linked motion (2 elements):**
- `Media` `parallax` over scrollY 0→6463px
- `Image` `parallax` over scrollY 0→6463px
- parallax: bind translateY to scrollYProgress with negative multiplier (e.g. `useTransform(p, [0,1], ['0%','-30%'])`)

**Paragraphs:**
- "(01)" — 12px / rgb(255, 255, 255)
- "Branding" — 12px / rgb(255, 255, 255)
- "Development" — 12px / rgb(255, 255, 255)
- "Box mode" — 12px / rgb(255, 255, 255)
- "2026" — 12px / rgb(255, 255, 255)
- "Portfolio" — 12px / rgb(255, 255, 255)
- "(02)" — 12px / rgb(255, 255, 255)
- "Web design" — 12px / rgb(255, 255, 255)

**Links:** `(01)BrandingDevelopmentBox mode2026Portfolio` · `(02)Web designDevelopmentNomad Stays2026Portfolio` · `(03)Web designBrandingWe run brand2026Portfolio`

**Images (4):**
- medium, 375×800 → `assets/images/dd8ffccf-RFACYseyJUnIgKpC8Ji85GEz4.avif`
- medium, 335×193 → `assets/images/dd8ffccf-RFACYseyJUnIgKpC8Ji85GEz4.avif`
- medium, 375×800 → `assets/images/73100a27-qtQPMLsOZSfMrr1H8paEqfCmqjQ.avif`
- medium, 335×193 → `assets/images/73100a27-qtQPMLsOZSfMrr1H8paEqfCmqjQ.avif`

**CSS background-image urls:**
- on `div.`: `assets/images/1dae10b6-rR6HYXBrMmX4cRpXfXUOvpvpB0.png`

### 5. `05-number`
*framer name: Number*
**Background:** `rgb(233, 233, 233)`

- screenshot (desktop): `screenshots/sections/05-number-desktop.png`
- screenshot (tablet): `screenshots/sections/05-number-tablet.png`
- screenshot (mobile): `screenshots/sections/05-number-mobile.png`
- dom subtree: `dom/sections/05-number.html`
- structural layout tree: `content/layouts.json` → find `"slug": "05-number"`

**Motion (114 animated · 2 fired during scroll):**
- defaults: 600ms × `ease`
- section enters on scroll: fade-up, ~600ms, easing `ease`
- 6 hover state(s): opacity (timing typically 0s ease)

**Hover states (6):**
- "Our ReviewsOur Reviews" — changes: opacity — 0s `ease`
- "Our ReviewsOur Reviews" — changes: opacity — 0s `ease`
- "Start a ProjectStart a Project" — changes: opacity — 0s `ease`
- "Start a ProjectStart a Project" — changes: opacity — 0s `ease`
- `svg:nth-child(3)` — changes: opacity — 0s `ease`
- `svg:nth-child(3)` — changes: opacity — 0s `ease`

**Headings:**
- h2: "Built onreputation" — 52px / 600 / rgb(11, 11, 11) / family: `Geist`

**Paragraphs:**
- "Why us?" — 12px / rgba(11, 11, 11, 0.6)
- "Average client rating on Google & Clutch" — 13px / rgb(255, 255, 255)
- "Our Reviews" — 13px / rgb(255, 255, 255)
- "Our Reviews" — 13px / rgb(255, 255, 255)
- "Business comes fromdirect referrals" — 13px / rgb(255, 255, 255)
- "Start a Project" — 13px / rgb(11, 11, 11)
- "Start a Project" — 13px / rgb(11, 11, 11)

**Links:** `Our ReviewsOur Reviews` · `Start a ProjectStart a Project`

**Images (1):**
- small, 100×100 → `assets/images/33e981b7-zEI0hdyA7XwBgF3OgjoRGPVMk.avif`

**Inline SVGs:** 3 (full markup in `content/sections.json`)

### 6. `06-desktop`
*framer name: Phone*
**Background:** `rgb(11, 11, 11)`

- screenshot (desktop): `screenshots/sections/06-desktop-desktop.png`
- screenshot (tablet): `screenshots/sections/06-desktop-tablet.png`
- screenshot (mobile): `screenshots/sections/06-desktop-mobile.png`
- dom subtree: `dom/sections/06-desktop.html`
- structural layout tree: `content/layouts.json` → find `"slug": "06-desktop"`

**Motion (200 animated · 4 fired during scroll):**
- defaults: 500ms × `ease`
- stagger group: 4 items, 70ms step, 500ms each, easing `cubic-bezier(0.68, 0, 0, 1)`

**Paragraphs:**
- "Services" — 12px / rgba(255, 255, 255, 0.6)
- "Every project starts with understanding how your customers make decisions — and what's stopping them from making one right now." — 22px / rgb(255, 255, 255)
- "Strategy & Research" — 16px / rgb(255, 255, 255)
- "Price: from" — 14px / rgba(255, 255, 255, 0.6)
- "$2,900" — 16px / rgb(255, 255, 255)
- "Matter Studio opens every project with an audit of your current customer journey. We identify the moments where users lose context or delay a decision, then restructure the flow so each next step feels like the obvious thing to do. Nbehavioral patterns backed by data." — 14px / rgba(255, 255, 255, 0.6)
- "This approach reduces drop-offs before design even begins. It builds an environment where choosing you becomes the path of least resistance for your customer." — 14px / rgba(255, 255, 255, 0.6)
- "Design & Prototyping" — 16px / rgb(255, 255, 255)

**CSS background-image urls:**
- on `div.`: `assets/images/fb56afed-V4ZkWaLPRZ6Dp0De8M0jUyQIc.avif`
- on `div.`: `assets/images/1dae10b6-rR6HYXBrMmX4cRpXfXUOvpvpB0.png`
- on `div.`: `assets/images/11ac623b-R8DWarznw4xTxUguf9qS1vaU0A.avif`
- on `div.`: `assets/images/318c972b-lcNzeG9RhgOhjPwtCyEu0UULtC0.avif`
- on `div.`: `assets/images/ef8482fe-iKu3BZinxyUoaGwZRZSSbtwnugk.avif`

### 7. `07-numbers`
*framer name: Numbers*
**Background:** `rgb(255, 69, 0)`

- screenshot (desktop): `screenshots/sections/07-numbers-desktop.png`
- screenshot (tablet): `screenshots/sections/07-numbers-tablet.png`
- screenshot (mobile): `screenshots/sections/07-numbers-mobile.png`
- dom subtree: `dom/sections/07-numbers.html`
- structural layout tree: `content/layouts.json` → find `"slug": "07-numbers"`

**Motion (111 animated · 6 fired during scroll):**
- defaults: 600ms × `ease`
- stagger group: 6 items, 80ms step, 600ms each, easing `cubic-bezier(0.68, 0, 0, 1)`
- **labels (small/uppercase):** `shipped` · `conversion lift` · `meaningful action` · `direct referrals` · `We don't chase volume` · `measurable difference`

**Headings:**
- h2: "Every result here started with a problem worth solving." — 52px / 600 / rgb(255, 255, 255) / family: `Geist`

**Paragraphs:**
- "How we do it" — 12px / rgba(255, 255, 255, 0.7)
- "Projects shipped with measurable conversion lift" — 12px / rgba(255, 255, 255, 0.7)
- "Average time to firstmeaningful action on our sites" — 12px / rgba(255, 255, 255, 0.7)
- "Of clients come fromdirect referrals" — 12px / rgba(255, 255, 255, 0.7)
- "We don't chase volume. We take on projects where our process can make a measurable difference. Most clients stay for years." — 12px / rgba(255, 255, 255, 0.6)
- "Jennifer Peterson" — 14px / rgb(255, 255, 255)
- "Head of Sales at" — 11px / rgb(255, 255, 255)
- "Mattis®" — 13px / rgb(255, 255, 255)

**Images (1):**
- small, 50×50 → `assets/images/7b2435d0-wlJMtkRVckBTirLzGQd8qmCMDw.avif`

### 8. `08-desktop`
*framer name: Phone*
**Background:** `rgb(233, 233, 233)`

- screenshot (desktop): `screenshots/sections/08-desktop-desktop.png`
- screenshot (tablet): `screenshots/sections/08-desktop-tablet.png`
- screenshot (mobile): `screenshots/sections/08-desktop-mobile.png`
- dom subtree: `dom/sections/08-desktop.html`
- structural layout tree: `content/layouts.json` → find `"slug": "08-desktop"`

**Motion (159 animated · 2 fired during scroll):**
- defaults: 600ms × `ease`
- section enters on scroll: fade-up, ~600ms, easing `ease`

**Headings:**
- h2: "Before weget started." — 52px / 600 / rgb(11, 11, 11) / family: `Geist`

**Paragraphs:**
- "FAQ" — 12px / rgba(11, 11, 11, 0.6)
- "Do you write the copy or do I need to provide it?" — 11px / rgba(11, 11, 11, 0.6)
- "We can handle it both ways. You can provide your own content, or our copywriters can craft professional, SEO-optimized copy tailored specifically to your brand and goals." — 18px / rgb(11, 11, 11)
- "Can I see the design before you build it?" — 11px / rgba(11, 11, 11, 0.6)
- "Absolutely. We don't start the development phase until you have reviewed and fully approved the high-fidelity design mockups in Figma." — 18px / rgb(11, 11, 11)
- "What happens after launch?" — 11px / rgba(11, 11, 11, 0.6)
- "We don’t just disappear. We provide post-launch technical support, training for your team on how to manage the site, and options for ongoing maintenance and scaling." — 18px / rgb(11, 11, 11)
- "What if I'm not happy with the result?" — 11px / rgba(11, 11, 11, 0.6)

**Links:** `Ask a questionAsk a question`

### 9. `09-quote-pricing`
*framer name: Quote + Pricing*
**Background:** `rgb(11, 11, 11)`

- screenshot (desktop): `screenshots/sections/09-quote-pricing-desktop.png`
- screenshot (tablet): `screenshots/sections/09-quote-pricing-tablet.png`
- screenshot (mobile): `screenshots/sections/09-quote-pricing-mobile.png`
- dom subtree: `dom/sections/09-quote-pricing.html`
- structural layout tree: `content/layouts.json` → find `"slug": "09-quote-pricing"`

**Motion (134 animated · 0 fired during scroll):**

**Headings:**
- h2: "Pricing." — 52px / 600 / rgb(255, 255, 255) / family: `Geist`

**Paragraphs:**
- "Anna Schneider" — 14px / rgb(255, 255, 255)
- "Head of Sales at" — 11px / rgb(255, 255, 255)
- "Mattis®" — 13px / rgb(255, 255, 255)
- "“The hardest part of building a website isn't the code — it's knowing what to leave out. Every element that doesn't serve the visitor is working against you.”" — 22px / rgb(255, 255, 255)
- "Our team treats simplicity as a discipline, not a shortcut." — 12px / rgba(255, 255, 255, 0.6)
- "A solid site built on proven structure. Launch-ready, no extras." — 12px / rgba(255, 255, 255, 0.6)
- "Foundation" — 12px / rgb(11, 11, 11)
- "Growth" — 12px / rgb(255, 255, 255)

**Links:** `Get startedGet started`

**CSS background-image urls:**
- on `div.`: `assets/images/5f4227b1-ncY5akdtmiquhkDxINCBcqKRm8.avif`
- on `div.`: `assets/images/1dae10b6-rR6HYXBrMmX4cRpXfXUOvpvpB0.png`

**Inline SVGs:** 4 (full markup in `content/sections.json`)

### 10. `10-desktop`
*framer name: Phone*
**Background:** `rgb(233, 233, 233)`

- screenshot (desktop): `screenshots/sections/10-desktop-desktop.png`
- screenshot (tablet): `screenshots/sections/10-desktop-tablet.png`
- screenshot (mobile): `screenshots/sections/10-desktop-mobile.png`
- dom subtree: `dom/sections/10-desktop.html`
- structural layout tree: `content/layouts.json` → find `"slug": "10-desktop"`

**Motion (43 animated · 6 fired during scroll):**
- defaults: 400ms × `ease`
- stagger group: 4 items, 60ms step, 400ms each, easing `cubic-bezier(0.68, 0, 0, 1)`
- **labels (small/uppercase):** `results speak` · `something to add`

**Headings:**
- h2: "What our clients say." — 52px / 600 / rgb(11, 11, 11) / family: `Geist`

**Paragraphs:**
- "Client stories" — 12px / rgba(11, 11, 11, 0.6)
- "We let the results speak. But sometimes the people behind them have something to add." — 12px / rgba(11, 11, 11, 0.6)
- ""We launched in two weeks and had paying customers by week three. I've worked with agencies that took months to deliver half of this."" — 22px / rgb(11, 11, 11)
- "Sophie Andersen" — 14px / rgb(11, 11, 11)
- "Co-founder" — 12px / rgba(11, 11, 11, 0.6)

**Images (1):**
- medium, 335×335 → `assets/images/b0c2360d-mORiocPNTtVLJZs2cAljPc1iMeE.avif`

**CSS background-image urls:**
- on `div.`: `assets/images/b0c2360d-mORiocPNTtVLJZs2cAljPc1iMeE.avif`
- on `div.`: `assets/images/1dae10b6-rR6HYXBrMmX4cRpXfXUOvpvpB0.png`

### 11. `11-articles`
*framer name: Articles*
**Background:** `rgb(233, 233, 233)`

- screenshot (desktop): `screenshots/sections/11-articles-desktop.png`
- screenshot (tablet): `screenshots/sections/11-articles-tablet.png`
- screenshot (mobile): `screenshots/sections/11-articles-mobile.png`
- dom subtree: `dom/sections/11-articles.html`
- structural layout tree: `content/layouts.json` → find `"slug": "11-articles"`

**Motion (27 animated · 2 fired during scroll):**
- defaults: 600ms × `ease`
- section enters on scroll: fade-up, ~600ms, easing `ease`

**Scroll-linked motion (1 elements):**
- `Desktop` `parallax` over scrollY 9515→13207px
- parallax: bind translateY to scrollYProgress with negative multiplier (e.g. `useTransform(p, [0,1], ['0%','-30%'])`)

**Headings:**
- h2: "News andupdates." — 52px / 600 / rgb(11, 11, 11) / family: `Geist`

**Paragraphs:**
- "See more" — 12px / rgb(255, 255, 255)
- "See more" — 12px / rgb(255, 255, 255)
- "Why most redesigns fail — and what to do instead" — 16px / rgb(11, 11, 11)
- "Mar 31, 2026" — 12px / rgba(11, 11, 11, 0.6)
- "How to write a landing page that actually converts" — 16px / rgb(11, 11, 11)
- "Mar 31, 2026" — 12px / rgba(11, 11, 11, 0.6)
- "How we cut bounce rate by 34% with one layout change" — 16px / rgb(11, 11, 11)
- "Mar 30, 2026" — 12px / rgba(11, 11, 11, 0.6)

**Links:** `See moreSee more` · `Why most redesigns fail — and what to do insteadMar 31, 2026` · `How to write a landing page that actually convertsMar 31, 2026` · `How we cut bounce rate by 34% with one layout changeMar 30, 2026` · `Small defaults, big outcomes: lessons from behavioral designMar 25, 2026`

**Images (4):**
- medium, 335×431 → `assets/images/19eb4c1f-LPSVulPRLpcRP2J08Ln0raAcQ.avif`
- small, 50×50 → `assets/images/471c2432-4eISosOoYjMJ3exo170tf63A0Z4.avif`
- medium, 335×507 → `assets/images/66beabc8-kM932F9EcDwrzgr753VM8bb6pIg.avif`
- medium, 335×296 → `assets/images/8d6bd7ab-MF8lvEusopYl3xxox4RCKrziJ0c.avif`

**CSS background-image urls:**
- on `div.`: `assets/images/19eb4c1f-LPSVulPRLpcRP2J08Ln0raAcQ.avif`
- on `div.`: `assets/images/1dae10b6-rR6HYXBrMmX4cRpXfXUOvpvpB0.png`
- on `div.`: `assets/images/66beabc8-kM932F9EcDwrzgr753VM8bb6pIg.avif`
- on `div.`: `assets/images/8d6bd7ab-MF8lvEusopYl3xxox4RCKrziJ0c.avif`

**Inline SVGs:** 1 (full markup in `content/sections.json`)

## Section Transitions (the choreography between sections)

> Real "Framer feel" lives at section boundaries: bg cross-fades, pin handoffs, exit/enter sequences. These are JS-driven (framer-motion `useScroll` / GSAP `ScrollTrigger.scrub`), not discrete CSS animations — easy to miss if you only look at per-section motion.

### 01-hero → 02-about
*bg rgb(255, 255, 255) → rgb(255, 69, 0), 10 pinned/scrub bridge, 2 exiting, 5 entering*
- scroll window: 200→1600px
- 🎨 **bg crossfade**: `rgb(255, 255, 255)` → `rgb(255, 69, 0)` over 1400px
- 🌉 **bridging** (pinned/scrub spanning the boundary):
  - `Closed` [pinned] — "MenuHomeWorksAboutBlogContactContacthell"
  - `Navigation Menu` [pinned] — "HomeWorksAboutBlogContact"
  - `Desktop` [pinned] — "START A PROJECTSTART A PROJECT"
  - `Closed` [pinned]
- ⬆ **exiting** (section A elements leaving):
  - `Container` [scroll-translated] — "(Est. 2019 — Version 1.0.4)Mattis® studi"
  - `BG` [scroll-translated]
- ⬇ **entering** (section B elements arriving):
  - `Media` [parallax]
  - `Image` [parallax]
  - `Media` [parallax]
  - `Media` [parallax]
  - `Image` [parallax]

### 02-about → 03-showreel
*bg rgb(255, 69, 0) → rgb(233, 233, 233), 10 pinned/scrub bridge, 2 exiting, 5 entering*
- scroll window: 1052→2452px
- 🎨 **bg crossfade**: `rgb(255, 69, 0)` → `rgb(233, 233, 233)` over 1400px
- 🌉 **bridging** (pinned/scrub spanning the boundary):
  - `Closed` [pinned] — "MenuHomeWorksAboutBlogContactContacthell"
  - `Navigation Menu` [pinned] — "HomeWorksAboutBlogContact"
  - `Desktop` [pinned] — "START A PROJECTSTART A PROJECT"
  - `Closed` [pinned]
- ⬆ **exiting** (section A elements leaving):
  - `Media` [parallax]
  - `Image` [parallax]
- ⬇ **entering** (section B elements arriving):
  - `Media` [parallax]
  - `Media` [parallax]
  - `Image` [parallax]
  - `Container` [scroll-translated] — "(Est. 2019 — Version 1.0.4)Mattis® studi"
  - `BG` [scroll-translated]

### 03-showreel → 04-works
*10 pinned/scrub bridge, 1 exiting, 6 entering*
- scroll window: 1739→3139px
- 🌉 **bridging** (pinned/scrub spanning the boundary):
  - `Closed` [pinned] — "MenuHomeWorksAboutBlogContactContacthell"
  - `Navigation Menu` [pinned] — "HomeWorksAboutBlogContact"
  - `Desktop` [pinned] — "START A PROJECTSTART A PROJECT"
  - `Closed` [pinned]
- ⬆ **exiting** (section A elements leaving):
  - `Media` [parallax]
- ⬇ **entering** (section B elements arriving):
  - `Media` [parallax]
  - `Image` [parallax]
  - `Media` [parallax]
  - `Image` [parallax]
  - `Container` [scroll-translated] — "(Est. 2019 — Version 1.0.4)Mattis® studi"
  - `BG` [scroll-translated]

### 04-works → 05-number
*10 pinned/scrub bridge, 2 exiting, 3 entering*
- scroll window: 4439→5839px
- 🌉 **bridging** (pinned/scrub spanning the boundary):
  - `Closed` [pinned] — "MenuHomeWorksAboutBlogContactContacthell"
  - `Navigation Menu` [pinned] — "HomeWorksAboutBlogContact"
  - `Desktop` [pinned] — "START A PROJECTSTART A PROJECT"
  - `Closed` [pinned]
- ⬆ **exiting** (section A elements leaving):
  - `Media` [parallax]
  - `Image` [parallax]
- ⬇ **entering** (section B elements arriving):
  - `Media` [parallax]
  - `Image` [parallax]
  - `Media` [parallax]

### 05-number → 06-desktop
*bg rgb(233, 233, 233) → rgb(11, 11, 11), 10 pinned/scrub bridge, 3 entering*
- scroll window: 5280→6680px
- 🎨 **bg crossfade**: `rgb(233, 233, 233)` → `rgb(11, 11, 11)` over 1400px
- 🌉 **bridging** (pinned/scrub spanning the boundary):
  - `Closed` [pinned] — "MenuHomeWorksAboutBlogContactContacthell"
  - `Navigation Menu` [pinned] — "HomeWorksAboutBlogContact"
  - `Desktop` [pinned] — "START A PROJECTSTART A PROJECT"
  - `Closed` [pinned]
- ⬇ **entering** (section B elements arriving):
  - `Media` [parallax]
  - `Media` [parallax]
  - `Image` [parallax]

### 06-desktop → 07-numbers
*bg rgb(11, 11, 11) → rgb(255, 69, 0), 10 pinned/scrub bridge*
- scroll window: 6559→7959px
- 🎨 **bg crossfade**: `rgb(11, 11, 11)` → `rgb(255, 69, 0)` over 1400px
- 🌉 **bridging** (pinned/scrub spanning the boundary):
  - `Closed` [pinned] — "MenuHomeWorksAboutBlogContactContacthell"
  - `Navigation Menu` [pinned] — "HomeWorksAboutBlogContact"
  - `Desktop` [pinned] — "START A PROJECTSTART A PROJECT"
  - `Closed` [pinned]

### 07-numbers → 08-desktop
*bg rgb(255, 69, 0) → rgb(233, 233, 233), 10 pinned/scrub bridge*
- scroll window: 7382→8782px
- 🎨 **bg crossfade**: `rgb(255, 69, 0)` → `rgb(233, 233, 233)` over 1400px
- 🌉 **bridging** (pinned/scrub spanning the boundary):
  - `Closed` [pinned] — "MenuHomeWorksAboutBlogContactContacthell"
  - `Navigation Menu` [pinned] — "HomeWorksAboutBlogContact"
  - `Desktop` [pinned] — "START A PROJECTSTART A PROJECT"
  - `Closed` [pinned]

### 08-desktop → 09-quote-pricing
*bg rgb(233, 233, 233) → rgb(11, 11, 11), 10 pinned/scrub bridge, 2 entering*
- scroll window: 8118→9518px
- 🎨 **bg crossfade**: `rgb(233, 233, 233)` → `rgb(11, 11, 11)` over 1400px
- 🌉 **bridging** (pinned/scrub spanning the boundary):
  - `Closed` [pinned] — "MenuHomeWorksAboutBlogContactContacthell"
  - `Navigation Menu` [pinned] — "HomeWorksAboutBlogContact"
  - `Desktop` [pinned] — "START A PROJECTSTART A PROJECT"
  - `Closed` [pinned]
- ⬇ **entering** (section B elements arriving):
  - `User Image` [parallax] — "Jennifer Peterson"
  - `Desktop` [parallax] — "Send messageSend message"

### 09-quote-pricing → 10-desktop
*bg rgb(11, 11, 11) → rgb(233, 233, 233), 10 pinned/scrub bridge, 12 entering*
- scroll window: 9659→11059px
- 🎨 **bg crossfade**: `rgb(11, 11, 11)` → `rgb(233, 233, 233)` over 1400px
- 🌉 **bridging** (pinned/scrub spanning the boundary):
  - `Closed` [pinned] — "MenuHomeWorksAboutBlogContactContacthell"
  - `Navigation Menu` [pinned] — "HomeWorksAboutBlogContact"
  - `Desktop` [pinned] — "START A PROJECTSTART A PROJECT"
  - `Closed` [pinned]
- ⬇ **entering** (section B elements arriving):
  - `User Image` [parallax] — "Jennifer Peterson"
  - `Darken` [parallax]
  - `Quote` [parallax] — "I'll personally review your brief and ge"
  - `Contact Info` [parallax] — "Contact+1 (555) 400 0123hello@mattistudi"
  - `Contact Details` [parallax] — "Contact+1 (555) 400 0123hello@mattistudi"
  - `Contact Info` [parallax] — "+1 (555) 400 0123hello@mattistudio.com"

### 10-desktop → 11-articles
*10 pinned/scrub bridge, 12 entering*
- scroll window: 10773→12173px
- 🌉 **bridging** (pinned/scrub spanning the boundary):
  - `Closed` [pinned] — "MenuHomeWorksAboutBlogContactContacthell"
  - `Navigation Menu` [pinned] — "HomeWorksAboutBlogContact"
  - `Desktop` [pinned] — "START A PROJECTSTART A PROJECT"
  - `Closed` [pinned]
- ⬇ **entering** (section B elements arriving):
  - `User Image` [parallax] — "Jennifer Peterson"
  - `Darken` [parallax]
  - `Quote` [parallax] — "I'll personally review your brief and ge"
  - `Contact Info` [parallax] — "Contact+1 (555) 400 0123hello@mattistudi"
  - `Contact Details` [parallax] — "Contact+1 (555) 400 0123hello@mattistudi"
  - `Contact Info` [parallax] — "+1 (555) 400 0123hello@mattistudio.com"

> 🔑 **How to implement**: wrap consecutive sections in a single `useScroll({target: containerRef})` and drive bg color via `useTransform(scrollYProgress, [0.4, 0.6], [fromBg, toBg])`. For bridging elements, use `position: sticky` + scale/opacity mapped to the same scroll progress. Full data in `motion/transitions.json`.


## Per-section build prompt (paste into Claude Code)

```text
Build the "01-hero" section.

Reference (look at all three viewports):
  - reference/mattis/screenshots/sections/01-hero-desktop.png
  - reference/mattis/screenshots/sections/01-hero-tablet.png
  - reference/mattis/screenshots/sections/01-hero-mobile.png

Source DOM subtree (for structure hints, do NOT copy verbatim):
  - reference/mattis/dom/sections/01-hero.html

Tokens to use:
  - reference/mattis/tokens/tokens.css

Motion specs (use EXACT durations/easings):
  - reference/mattis/motion/motion-specs.md

Stack: Next.js (App Router) + TypeScript + Tailwind CSS + Motion (framer-motion) + Lenis

Build, then take a screenshot of your output at 1440×900 and diff it against the desktop reference. Iterate until pixel-close. Then handle tablet (768) and mobile (390).
```

## Framer-tier polish checklist

- [ ] No "default" easings — every transition uses a specific cubic-bezier from `motion-specs.md`.
- [ ] Hero copy enters with word-by-word stagger (`staggerChildren: 0.1-0.15`).
- [ ] Section enters use `whileInView` with `viewport={{ once: true, margin: "-10%" }}`.
- [ ] Smooth scroll is wired (Lenis if the source uses it).
- [ ] All images are local (in `public/`), converted to webp.
- [ ] All fonts are self-hosted from `assets/fonts/` (don't rely on Framer's CDN).
- [ ] Hover states are 0.2-0.3s ease-out, not snappy/instant.
- [ ] Mobile layout actually works — not just a squished desktop.
- [ ] No console errors. No layout shift on load.