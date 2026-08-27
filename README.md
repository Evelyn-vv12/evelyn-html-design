# Evelyn HTML Design Skill

A personal visual design skill for generating HTML reports, dashboards, one-page presentations, and interactive pages in Evelyn's preferred visual language.

This repository is intended to be used **together with** structural HTML skills:

- `onepage` — narrative structure and chapter flow
- `show-html` — page patterns, components, and self-contained HTML
- `html-report` — interactive report behaviors
- `evelyn-html-design` — Evelyn's visual language: color, typography, spacing, cards, gradients, charts, and finishing rules

## Default visual direction

**Soft modern / restrained feminine / blush + lavender + periwinkle / premium calm**

The design should feel personal without becoming childish, overly decorative, or difficult to read.

Core palette:

| Token | Hex |
|---|---|
| Periwinkle | `#7C88BB` |
| Blush | `#E79798` |
| Petal | `#E2B9BD` |
| Mauve | `#B7728C` |
| Lavender | `#BDAABF` |
| Plum | `#3C2C40` |
| Ink | `#1B1117` |
| Canvas | `#F8F6FA` |

Default body typography:

- English: **Manrope**
- Chinese: **Noto Sans SC / PingFang SC**
- Editorial headings: **Cormorant Garamond / Noto Serif SC**
- Personal accent: **LXGW WenKai**

## Repository structure

```
.
├── SKILL.md
├── README.md
├── assets/
│   ├── theme.css
│   └── preview.html
├── references/
│   ├── color-system.md
│   ├── typography.md
│   ├── layout-rules.md
│   ├── components.md
│   └── illustration-system.md
└── examples/
    ├── report.html
    └── dashboard.html
```

## Usage

When generating HTML for Evelyn, apply this skill as the final design layer after deciding the content hierarchy.

Recommended workflow:

```
onepage
  ↓
show-html
  ↓
html-report (when interaction is needed)
  ↓
evelyn-html-design
```

If the user explicitly requests a different visual style for a specific artifact, that request overrides this skill for that artifact.

## Presentation default

For HTML used as a deck or report presentation, the default is **16:9 / 1920×1080**, one slide per frame. The canonical main character is the simple curly-haired blonde line-art girl, used as a compositional actor rather than a detached mascot. See `references/illustration-system.md`.

## Maintenance rule

This repository should be updated whenever Evelyn confirms a recurring preference about:

- color
- typography
- spacing
- card styling
- report density
- chart styling
- responsive behavior
- interaction
- visual do / don't rules
- presentation / PPT slide behavior
- recurring character / illustration rules

One-off visual requests should not automatically become permanent rules.
