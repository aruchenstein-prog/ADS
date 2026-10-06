# SOLUM: landing page

A single-page storefront concept for SOLUM, sneakers designed in Zürich. It's static HTML, CSS and JavaScript with no build step and no dependencies apart from Google Fonts.

## Run it

Open `index.html` in a browser, or serve the folder:

```sh
npx serve solum      # or: python3 -m http.server --directory solum
```

## Deploy

Upload the `solum/` folder as-is to any static host (Netlify, Vercel, Cloudflare Pages, GitHub Pages or plain hosting). Keep `index.html` and `img/` together.

Before launch:
- Point the footer links (Privacy, Terms, Imprint, Size guide, and so on) at real pages.
- Connect **Checkout** to the payment provider. The bag drawer currently keeps items in memory only.
- Connect the **Club** signup form to the newsletter tool. It validates and confirms, but doesn't send anything yet.
- Set `og:image` to an absolute URL once the domain is known.

## What's on the page

| Section | Notes |
|---|---|
| Intro curtain | Shown once per browser session. It is skipped for reduced-motion users and clears itself even if scripts fail. |
| Hero | Aster 2 with a live colourway picker, sizes and add to bag. |
| This season | Six products with filters, quick add, 3D tilt and glare. On phones it becomes a swipeable rail. |
| Campaign band | Full-bleed photo with parallax and a reveal wipe. |
| Two new shapes | Meridian and Tide viewer: 4 views, 4 colourways each, turntable, arrow keys and swipe. |
| Built in layers | Bento grid of specs with count-up numbers, plus the repair offer. |
| Collections / Journal | Photo tiles with wipe reveals and an "Explore / Read" cursor label. |
| Club | Newsletter signup with validation. |
| Bag + Search | Bag drawer (subtotal, free-shipping meter, remove items) and product search. |

## Editing

- **Colours and type:** CSS custom properties at the top of `<style>` (`--canvas`, `--ink`, `--ember`, `--volt`, …). Fonts are Archivo (display/UI) and Instrument Serif (accents).
- **Shoes** are inline SVG symbols, recoloured through CSS variables:
  - `#shoe` / `#shoe-trail` use `--s-upper`, `--s-over`, `--s-lining`, `--s-mid`, `--s-sole`, `--s-accent`, `--s-lace`.
  - `#mer-*` / `#tide-*` (side, top, sole, back) use `--m-base`, `--m-l1..l3`, `--m-mid`, `--m-sole`, `--m-pop`, `--m-lace`, `--m-collar`.
  - Colourways are defined in the `CW` object (hero) and the `MODELS` object (viewer) in the script.
- **Photos** are in `img/` as WebP; sources and licences are in `img/CREDITS.md`.

## Quality

- Works without JavaScript: every section's content is in the HTML, and scripts only add motion and interactivity.
- `prefers-reduced-motion` turns off the intro, parallax, tilt, magnetic buttons and reveals.
- Keyboard: skip link, visible focus, and Escape closes the menu, bag and search. The viewer works with arrow keys.
- Responsive from 360 px phones up to wide desktops, with no horizontal scrolling.
