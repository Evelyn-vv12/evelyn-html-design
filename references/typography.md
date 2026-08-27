# Typography

## Default preset — Soft Modern

Use for:
- reports
- dashboards
- weekly summaries
- data analysis
- operating reviews
- implementation pages

English:
```css
Manrope, Inter, ui-sans-serif, -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif
```

Chinese:
```css
"Noto Sans SC", "PingFang SC", "Microsoft YaHei", "Source Han Sans SC", sans-serif
```

Combined:
```css
Manrope, Inter, "Noto Sans SC", "PingFang SC", "Microsoft YaHei", "Source Han Sans SC", ui-sans-serif, -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif
```

## Editorial preset

Use for:
- report cover title
- brand narrative
- opening statement
- premium feature page
- short pull quote

English heading:
```css
"Cormorant Garamond", Georgia, "Times New Roman", serif
```

Chinese heading:
```css
"Noto Serif SC", "Songti SC", SimSun, serif
```

Body remains in Soft Modern.

## Personal accent

Use sparingly for:
- short note
- signature-like text
- quote
- one personal caption

```css
"LXGW WenKai", "Noto Serif SC", "KaiTi", serif
```

Do not use for:
- long body paragraphs
- dense cards
- tables
- metric labels

## Type scale

Recommended defaults:

| Role | Size |
|---|---|
| Body desktop | 16px |
| Body mobile | 15–16px |
| H1 | clamp(34px, 5vw, 64px) |
| H2 | clamp(24px, 3vw, 38px) |
| H3 | 18–22px |
| Eyebrow / label | 11–12px |
| Table / dense meta | 12–14px |

## Line height

Chinese-heavy body:
- 1.65–1.75

English-heavy body:
- 1.55–1.65

Headings:
- 1.02–1.28 depending on size

## Weight

Body:
- 400–500

Heading:
- 600–700

Editorial serif:
- 500–600 usually enough

Avoid very thin 300 weight for long Chinese content.

## Tracking

English headline:
`-0.02em` to `-0.035em`

Chinese headline:
`0` to `0.02em`

Body:
close to normal

Never apply uppercase transforms to Chinese.

## Numbers

For dashboards and metric-heavy reports:

```css
font-variant-numeric: tabular-nums;
```

Use tighter tracking on large metrics, but not on ordinary body numbers.
