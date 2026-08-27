---
name: evelyn-html-design
description: Apply Evelyn's personal visual design system to HTML reports, dashboards, one-page presentations, interactive reports, and web artifacts. Use together with onepage, show-html, or html-report whenever generating HTML for Evelyn unless a different visual style is explicitly requested. Default visual direction: soft modern, restrained feminine, blush pink + muted lavender/periwinkle, deep plum contrast, comfortable Chinese/English typography, restrained gradients, generous spacing, rounded cards, subtle glow, and clear information hierarchy.
license: private
metadata:
  owner: Evelyn
  version: "1.1.0"
---

# Evelyn HTML Design

This skill is a **visual design layer**. It does not replace content planning or report structure.

## Responsibility split

Use the HTML stack in this order:

1. `onepage` — decide audience, page mode, narrative structure, chapter flow, and information hierarchy.
2. `show-html` — choose page patterns, visual components, diagrams, tables, dashboard structures, and self-contained HTML behavior.
3. `html-report` — add interactive report behaviors when useful: tabs, filters, dark mode, sortable tables, charts, TOC, search.
4. `evelyn-html-design` — apply Evelyn's visual language: palette, typography, spacing, cards, gradients, chart colors, interaction tone, and finishing.

Do not let visual styling weaken the report's information hierarchy.

## Default visual character

Keywords:

**soft modern / dreamy editorial / restrained feminine / periwinkle glow / blush light / premium calm**

The reference mood combines:
- warm blush highlights
- cool lavender and periwinkle
- deep plum / near-black contrast
- soft atmospheric glow
- refined visual softness without becoming childish

The goal is **not** "make everything pink". The goal is a calm, polished visual system where pink adds warmth and purple-blue adds balance.

## Read these references

Before producing final HTML, use:

- `references/color-system.md` — palette, gradients, semantic color rules.
- `references/typography.md` — Chinese/English fonts, type scale, line height, bilingual rules.
- `references/layout-rules.md` — spacing, density, responsive behavior, hero and page layout.
- `references/components.md` — cards, buttons, badges, tables, charts, interactions.
- `references/illustration-system.md` — Evelyn's canonical character system, supporting dog, placement logic, and illustration do/don't rules.
- `assets/theme.css` — reusable CSS variables and base styling.

Use `assets/preview.html` as a compact style reference.

## Core palette

- Periwinkle: `#7C88BB`
- Blush: `#E79798`
- Petal: `#E2B9BD`
- Mauve: `#B7728C`
- Lavender: `#BDAABF`
- Plum: `#3C2C40`
- Ink: `#1B1117`
- Canvas: `#F8F6FA`
- Card: `#FFFFFF`

Primary gradient:

`linear-gradient(135deg, #E7AFB7 0%, #C4B2CC 48%, #8793C4 100%)`

Recommended visual balance:
- 60–70% neutral canvas / white card space
- 20–30% pale pink / lavender / periwinkle surfaces
- 5–10% stronger accent color

Do not use gradients on every card.

## Typography

### Default: Soft Modern

Use for reports, dashboards, analysis, work summaries, operating pages.

English:
`Manrope, Inter, ui-sans-serif, -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif`

Chinese:
`"Noto Sans SC", "PingFang SC", "Microsoft YaHei", "Source Han Sans SC", sans-serif`

Combined body stack:
`Manrope, Inter, "Noto Sans SC", "PingFang SC", "Microsoft YaHei", "Source Han Sans SC", sans-serif`

### Editorial Accent

Use for premium cover titles, brand narratives, opening statements, short feature headings.

English:
`"Cormorant Garamond", Georgia, "Times New Roman", serif`

Chinese:
`"Noto Serif SC", "Songti SC", SimSun, serif`

Keep body copy in the default sans stack.

### Personal Accent

For short personal notes, quotes, captions, or signature-like text:

`"LXGW WenKai", "Noto Serif SC", "KaiTi", serif`

Never use this for long body copy, dense reports, or tables.

## Presentation mode

When HTML is used as a presentation or report deck, default to **PPT-style slides** rather than a long webpage.

- default canvas: **16:9**
- canonical working size: **1920×1080**
- one slide = one fixed presentation frame
- do not default to long-scroll layouts for presentation work
- each slide should have one dominant message and a clear visual hierarchy
- characters and doodles must participate in the composition, not sit as detached decoration

See `references/layout-rules.md` and `references/illustration-system.md`.

## Canonical character system

The default main character is Evelyn's **simple curly-haired girl line-art character**.

Canonical traits:
- short-to-medium curly blonde bob
- simple cute line-art face; expressive but not oversized glossy "Powerpuff" eyes
- clean, light sketch treatment with minimal fill and minimal shading
- pleated skirt
- elegant high heels
- coordinated fitted short-sleeve blouse / top, tucked in
- feminine, smart, light, and presentation-friendly
- no heavy solid black clothing blocks
- no bow-covered shoes / chunky cartoon boots
- no realistic rendering

The character is a **layout actor**, not a sticker:
- lean on typography
- touch or point to a keyword, number, chart, or process step
- sit or stand on a baseline
- bridge two information areas
- visually anchor a conclusion

The small fluffy dog is a supporting character and should usually sit near the base of a composition, closing whitespace or supporting a warm / playful moment.

## Visual rules

Prefer:
- strong hierarchy
- calm whitespace
- rounded but not bubbly cards
- subtle mauve / plum borders
- broad low-contrast shadows
- one focal gradient or glow per section
- data-first layouts for work reports
- semantic chart colors
- restrained hover motion

Avoid:
- neon magenta
- cyberpunk purple
- heavy glassmorphism
- all-pink card grids
- decorative gradients behind dense tables
- excessive full-pill UI
- tiny gray text
- heavy drop shadows
- constant floating or pulsing animation
- sacrificing information density for decoration

## Bilingual readability

For Chinese-heavy content:
- body line height: 1.65–1.75
- body font weight: 400–500
- heading font weight: 600–700
- do not compress Chinese tracking
- avoid overly narrow text columns

For English:
- headings may use `letter-spacing: -0.02em`
- body tracking should remain close to normal

For mixed CN/EN:
- default to one shared sans stack in body text
- keep English acronyms aligned to Chinese baseline and size
- do not mechanically uppercase Chinese labels

## Interaction

- hover lift: 1–2px maximum
- transition: about 160–220ms
- focus rings must remain visible
- respect `prefers-reduced-motion`
- interaction should help scan or navigate, not decorate

## Dark mode

When useful:
- background: `#171219`
- surface: `#211923`
- text: `#F6EEF5`
- muted: `#C9BBC8`
- pink accent: `#E5A1B2`
- periwinkle accent: `#A9B3E1`

Dark mode should feel plum / ink, not pure black.

## Font loading

If the parent artifact must be fully offline or zero-dependency:
- use system fallbacks only.

If external font loading is allowed:
- default: Manrope + Noto Sans SC
- editorial option: Cormorant Garamond + Noto Serif SC
- optional personal accent: LXGW WenKai

The page must remain readable when web fonts fail.

## Final quality check

Before delivery verify:

1. The page's information hierarchy is clear before the styling is noticed.
2. Pink/purple is a visual language, not the entire page.
3. Chinese and English both render comfortably.
4. Body text is readable at desktop and 375px mobile widths.
5. Gradients/glow never reduce contrast.
6. Tables and charts stay legible.
7. The page feels soft, modern, refined, and personal — not childish or neon.
8. Mobile layout has no horizontal overflow except intentional scrollable tables.
9. Repeated preferences belong in this skill; one-off requests do not.
10. Presentation HTML defaults to 16:9 / 1920×1080 unless the task explicitly requires another ratio.
11. The main character must feel integrated with the message or layout; avoid detached corner placement.
12. The canonical girl retains the approved short curly hair + pleated skirt + high heels + light blouse styling unless a task explicitly calls for another outfit.
