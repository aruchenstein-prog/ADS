# Working in this repository

This repo holds website projects built for the owner. Read this before starting any task. It records the owner's standing preferences; follow them without being asked again.

## The owner and how to talk to them

- Writes mostly in **German** (casual, sometimes English). **Reply in the language of their last message**, in short, plain language without jargon. Explain what was done and what they need to do, step by step.
- Texts that go **on websites or social posts** are in **English** unless asked otherwise.
- Wants work that is **client-ready**: polished, tested, nothing broken, nothing half-finished. "Make it very nice" means premium agency quality, not a template.
- Prefers **free tools**. Never spend money or credits on their behalf; if a tool costs money, say so and offer a free route.
- Values honesty: say clearly when something can't be done, when a tool's output is not good enough, or when a fix was only cosmetic.
- When they share work-in-progress images, check them carefully and say what's good and what's off before using them.

## Projects

- `solum/`: **SOLUM**, a fictional premium sneaker brand ("designed in Zürich"). Single-page storefront and the owner's **portfolio / demo ad**. The quality reference for all new work. See `solum/README.md`.
  - `solum/promo/`: LinkedIn kit (4:5 video, carousel PDF, post texts in `LINKEDIN.md`, reach plan in `REICHWEITE.md`).
  - `solum/img/neu/PROMPTS.md`: image prompts the owner runs in Perchance.
- `schwung/`: **schwung**, the owner's own design studio ("Websites that move", Zürich): brand kit in `schwung/brand/` (logo SVGs, social media assets, brand board), brand rules and profile texts in `schwung/BRAND.md`, studio one-pager `schwung/index.html` with SOLUM as the case study. Use its logo, colours (Ink #0D0D0C, Paper #F2EFE9, Schwung Blue #3D2BFF) and tone for anything about the studio.
- `aml-revisions/`: landing page for the owner's father's real company (AML Revisions AG, audit firm for asset managers). **Do not change it unless the owner explicitly asks for that page.** Never apply SOLUM work (animations, styles, promo) to it. Audience: older clients, so calm, text-first, large type, no flashy motion.
- `waymark/`: earlier concept page.
- `design-md/`: design reference library used by the `design-references` skill.

## How the owner likes new pages built

1. **Design process:** load the `design-references` skill, pick 2–3 fitting references from `design-md/INDEX.md`, and synthesize an original system. For premium or brand work, also follow `high-end-visual-design`. Finish with a `web-design-guidelines` review (accessibility, focus, forms).
2. **Look and feel (SOLUM style):**
   - Warm canvas instead of white, one signal accent colour used sparingly.
   - Huge condensed display type (Archivo, `font-stretch: 62%`) mixed with an italic serif accent word (Instrument Serif).
   - Pill buttons with a nested arrow circle, framed ("double-bezel") cards, and a floating island nav.
   - Generous spacing, a subtle paper grain, and no generic template look.
3. **Motion that feels premium:**
   - A one-time intro, a scroll progress line, and word-by-word heading reveals.
   - Photo wipe reveals and light parallax (clamp values so nothing stays offset).
   - Magnetic buttons, 3D card tilt with glare, a cursor label on tiles, fly-to-bag and count-up numbers.
   - Everything respects `prefers-reduced-motion`, and only `transform`/`opacity` are animated.
4. **Things must actually work:** no dead buttons. Bag (with subtotal), search, filters, colour pickers, forms with validation and a mobile menu should all function.
5. **Content must always show.** The owner's preview viewer can pause animations. Keep failsafes: the intro is removed by a timer, content shows if transitions are frozen or scripts fail, and the full HTML content is present without JS (prefill anything JS would render).

## Images

- **Real-looking imagery over drawings** wherever it's a product or mood shot. Drawings (recolourable inline SVG) only where photos can't do the job, such as multi-view viewers or labelled diagrams.
- **Image generation:**
  - **Perchance** (free): the owner generates images manually from prompts I write (add them to a `PROMPTS.md` with exact filenames), then uploads them. Images they send *while I'm still working* may arrive only as chat previews, not files; if so, ask them to resend.
  - **Higgsfield** is connected but the account has **0 credits**: don't use it for generation unless they say they bought credits.
  - **Pollinations** anonymous tier is not good enough (watermark, weak model). **Hugging Face** (free token as secret `HF_TOKEN`, domain `router.huggingface.co`) is the automatic option if they set it up.
- **Stock photos:** Pexels (`images.pexels.com`) and Unsplash (`images.unsplash.com`) CDNs are allowed; their search pages are blocked. Find IDs via web search, download candidates, and **look at every image at full resolution before using it**.
- **No third-party brand logos or recognisable designs** (Nike swoosh, adidas stripes, Vans, Converse star, Air Max 95, Yeezy…) on a fictional brand's page. Zoom into tongue, heel and side to check.
- **Cut-outs:** remove backgrounds with `rembg` (install in a venv in the scratchpad: `pip install "rembg[cpu]"`, model `isnet-general-use`), retouch small artefacts with PIL, save as transparent WebP with prefix `cut-`. Generated mood images use prefix `gen-`.
- Store images resized as WebP in the project's `img/` folder, lazy-loaded with width and height, and list every source in `img/CREDITS.md`. Remove replaced images from the repo.

## Checking and delivering

- **Full QA before saying it's done** (Playwright, Chromium preinstalled; `NODE_PATH=$(npm root -g) node script.js`):
  - widths 360, 390, 768, 1024, 1280, 1440 and 1920: no horizontal scroll, all images load, all sections visible;
  - click every interaction (nav, menu, swatches, sizes, filters, every quick add, viewer views and colours, bag remove/checkout, search, forms);
  - reduced motion, paused/frozen animations, keyboard (skip link, Escape);
  - static checks: duplicate ids, broken anchors, missing alt/size, leftover names of removed products in text and meta tags;
  - look at viewport screenshots at the top of the page too (full-page screenshots can distort fixed and parallax elements).
- **Always send the owner a self-contained preview file**: HTML with every image embedded as a data URI, including image paths inside JavaScript strings, so it opens on its own in their app.
- **For publishing**, also send a ZIP of `index.html` + `img/` (without `img/neu/`) for Netlify Drop (app.netlify.com/drop).
- Commit with clear messages and push to the session's working branch. Mention anything that still needs real services (checkout, newsletter, legal pages).

## Promotion goals

- SOLUM is used as a **demo ad / portfolio piece on LinkedIn** (and Instagram etc.) to win web-design work and build reach. Keep it labelled as a **concept with a fictional brand**, and mention AI-generated product images openly.
- Promo assets live in `solum/promo/`. New formats (9:16 reel, 16:9, banners) should match the same look: warm canvas, condensed headline with an italic accent word, real site footage.
