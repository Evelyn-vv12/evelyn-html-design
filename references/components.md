# Components

## Cards

Default:
```css
background: #fff;
border: 1px solid rgba(60,44,64,.10);
border-radius: 20px;
box-shadow: 0 18px 52px rgba(60,44,64,.08);
```

Variants:
- neutral white
- pink wash
- lavender wash
- periwinkle wash

Use one tinted card to guide attention, not every card.

## Buttons

Primary:
- Plum `#3C2C40` or Periwinkle `#7C88BB`
- white text
- 12–14px radius
- 44px minimum height

Secondary:
- white/pale surface
- subtle plum border
- dark plum text

Default buttons are rounded rectangles, not full pills.

## Badges

- compact
- pale pink/lavender/periwinkle fill
- plum text
- use pills sparingly

Status badges must preserve semantic meaning.

## Tables

Preferred:
- white surface
- 12–14px outer radius
- pale lavender header
- subtle row separators
- nearly invisible zebra striping if needed
- sticky header for long tables
- sortable/filterable when interaction is useful

Avoid:
- dark decorative gradients behind tables
- excessive cell padding
- tiny low-contrast text

## Metrics

Large metric:
- strong plum/ink
- tabular numbers
- concise label
- optional blush/periwinkle delta indicator

Avoid making every metric card a different saturated color.

## Charts

Preferred brand series:
1. Periwinkle `#7C88BB`
2. Muted rose `#C8809A`
3. Soft violet `#9B82AE`
4. Petal `#D4A3AB`
5. Slate-periwinkle `#6F789F`

Use semantic red/amber/green where meaning requires it.

Chart background should remain neutral.

## Tabs and segmented controls

- pale neutral container
- active tab may use plum text + white/pale surface
- restrained shadow
- do not use saturated pink for every selected state

## Navigation / TOC

- compact
- quiet
- active section may use periwinkle or mauve
- avoid visually competing with report content

## Hover

Preferred:
```css
transform: translateY(-1px);
transition: transform 180ms ease, box-shadow 180ms ease;
```

Maximum lift: about 2px.

## Focus

Always provide visible `:focus-visible` styling.

Recommended focus color:
`rgba(124,136,187,.40)`

## Motion

- 160–220ms
- no constant floating/pulsing
- respect reduced motion
