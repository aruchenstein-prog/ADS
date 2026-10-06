---
name: design-references
description: Use the DESIGN.md reference library in design-md/ as inspiration when designing or restyling any UI (pages, components, landing pages, dashboards, artifacts). Picks 2-3 relevant references, extracts the principles that make them look good, and synthesizes an original design system for this project instead of copying any one site.
---

# Design references

`design-md/` holds ~70 `DESIGN.md` files, each a detailed analysis of a well-designed website: color roles, type scale, spacing, components, elevation, do's and don'ts. They are a **study library, not templates to clone**. The goal is to borrow *why* those sites look good and produce something original that fits this project.

## When to use

Any time you create or noticeably restyle UI: a new page, a landing page, a component set, a dashboard, an HTML artifact, or a "make this look better" request.

## Process

1. **Understand the brief.** What is the product, who uses it, what mood fits (calm/technical, warm/consumer, luxury/editorial, playful, data-dense)? If the project already has a `DESIGN.md` at its root or an existing visual style, that wins. Use references only to fill gaps.

2. **Pick 2-3 references** from `design-md/INDEX.md` (read the index, not every file). Choose for *fit with the brief*, and prefer a mix:
   - one that matches the overall mood,
   - one strong in the specific thing being built (e.g. pricing tables, dashboards, docs, marketing heroes),
   - optionally one contrasting reference for a single idea worth stealing.

3. **Read only the useful sections** of those files: usually Overview, Colors, Typography, Layout, Components, Do's and Don'ts. Skip the rest unless needed.

4. **Extract principles, not values.** Write down (briefly, for yourself) things like:
   - how many accent colors, and how sparingly they're used
   - type scale ratios, weights, letter-spacing habits on display vs body
   - spacing rhythm (e.g. 8px ladder, section padding)
   - radius / border / shadow philosophy
   - what the reference deliberately avoids

5. **Synthesize an original system** for this project: its own palette (new hues, same *role structure*), font choice from freely available fonts (Google Fonts etc.), spacing scale, radii, component treatments. Then build the UI with it.

6. **Briefly tell the user** which references informed the design and which ideas came from each (one line each).

## Rules

- **Never clone a brand.** Don't reuse a reference's exact brand colors as the main palette, its proprietary fonts, logos, product names, slogans, or signature motifs (e.g. Stripe's gradient mesh, Ferrari red, Apple's product-photo layouts) in a way that makes the result look like that company's site.
- Don't mix more than ~3 references. Too many sources produce mush. One coherent system beats a collage.
- Copy structure and discipline, not decoration: role-based color tokens, consistent scales, restraint with accents, and clear hierarchy are what transfer well.
- Respect accessibility while adapting: check text contrast (WCAG AA), visible focus states, sensible touch targets, and keep dark/light mode working if the project supports it.
- If the user names a reference ("make it feel like Linear"), lean on that one, but still produce an original identity unless they explicitly ask for a faithful recreation.
- Combine with other installed design skills (e.g. `design-taste-frontend`, `high-end-visual-design`, `web-design-guidelines` for a final review) when relevant.
