# Working in this repository

This repo holds website projects built for the owner. Read this before starting any design or web task.

## Projects

- `solum/`: **SOLUM**, a fictional premium sneaker brand ("designed in Zürich"). Single-page storefront, the reference for quality. See `solum/README.md`.
- `aml-revisions/`: landing page for the owner's father's real company (AML Revisions AG, an audit firm for asset managers). **Do not change it unless the owner explicitly asks for that page.** Never apply SOLUM work (animations, styles) to it. Its audience is older clients: calm, text-first, large type, no flashy motion.
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
   - Photo wipe reveals and light parallax.
   - Magnetic buttons, 3D card tilt with glare, a cursor label on tiles, fly-to-bag and count-up numbers.
   - Everything respects `prefers-reduced-motion`, and only `transform`/`opacity` are animated.
4. **Things must actually work:** no dead buttons. Bag, search, filters, colour pickers, forms with validation, and a mobile menu should all function.
5. **Content must always show.** The owner's preview viewer can pause animations. Keep failsafes: the intro is removed by a timer, content shows if transitions are frozen or scripts fail, and the full HTML content is present without JS.

## Images

- Pexels (`images.pexels.com`) and Unsplash (`images.unsplash.com`) image CDNs are allowed in this environment; their websites and search pages are blocked. Find photo IDs via web search, download candidates, and **look at every image before using it**.
- No visible third-party brand logos (Nike, adidas and so on) on a fictional brand's page.
- Never put a real company's product photo or recognisable design (for example an Air Max 95) on the page as our own. Use references as inspiration and draw original shoes as recolourable inline SVG.
- Store photos resized as WebP in the project's `img/` folder, lazy-loaded with width and height set, and list sources in `img/CREDITS.md`.

## Checking and delivering

- Verify with Playwright (Chromium is preinstalled; `NODE_PATH=$(npm root -g) node script.js`):
  - screenshots at 1440 px desktop and 390 px phone;
  - no horizontal scroll and no console errors;
  - click through every interaction;
  - also test reduced motion and paused animations.
- **Always send the owner a self-contained preview file**: the HTML with every image embedded as a data URI, so it opens on its own in their app. A plain `index.html` without its `img/` folder shows no photos.
- Commit with clear messages and push to the session's working branch.
- Explain results in short, plain English without jargon. Mention anything that still needs real services (checkout, newsletter, legal pages).
