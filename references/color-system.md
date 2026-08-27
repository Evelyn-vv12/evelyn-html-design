# Color System

## Core palette

| Token | Hex | Primary use |
|---|---|---|
| Periwinkle | #7C88BB | cool anchor, charts, active states |
| Blush | #E79798 | warm highlight, selected emphasis |
| Petal | #E2B9BD | pale warm surface |
| Mauve | #B7728C | secondary accent, labels |
| Lavender | #BDAABF | secondary cool surface |
| Plum | #3C2C40 | strong text, key controls |
| Ink | #1B1117 | primary body text |
| Canvas | #F8F6FA | page background |
| Card | #FFFFFF | main content surface |

Soft surface colors:
- pink wash: `#FBF2F5`
- lavender wash: `#F2F1F8`
- periwinkle wash: `#EEF0F8`
- plum wash: `#F4EFF4`

## Gradients

Primary gradient:

```css
linear-gradient(135deg, #E7AFB7 0%, #C4B2CC 48%, #8793C4 100%)
```

Hero atmospheric glow:

```css
radial-gradient(circle at 22% 20%, rgba(231,151,152,.34), transparent 34%),
radial-gradient(circle at 82% 8%, rgba(124,136,187,.34), transparent 38%)
```

Use gradients for:
- hero areas
- one major highlight
- compact accent bars
- selected chart emphasis

Do not use gradients:
- behind dense tables
- on every card
- as a substitute for hierarchy

## Balance

Default visual ratio:
- 60–70% neutral
- 20–30% pale tinted surfaces
- 5–10% stronger color

This keeps the page useful for work while preserving the personal style.

## Semantic colors

Brand colors must not replace semantic meaning.

Use clear semantic colors for:
- success
- warning
- danger
- neutral/inactive

Pink and purple may frame the status UI, but must not make error and success states ambiguous.

## Chart palette

Preferred series order:
1. `#7C88BB`
2. `#C8809A`
3. `#9B82AE`
4. `#D4A3AB`
5. `#6F789F`

For many categories, extend with neutrals rather than creating many near-identical pinks.

## Contrast

- primary text: Ink / Plum on light surfaces
- avoid pale pink text on white
- avoid lavender body text on light lavender surfaces
- use white text only on sufficiently dark plum/periwinkle surfaces
