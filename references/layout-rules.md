# Layout Rules

## Overall principle

Design for **fast comprehension first**.

The visual system should make a report feel personal and polished without making it less efficient.

## Page width

Typical report width:
- 1040–1180px

Dense dashboard:
- up to 1280px when needed

Reading-heavy report:
- 860–1040px

## Page padding

Desktop:
- 40–64px horizontal
- 48–80px vertical

Mobile:
- 18–20px horizontal
- 28–40px vertical

## Section rhythm

Typical spacing:
- hero → first section: 28–40px
- section → section: 32–48px
- heading → content: 14–22px
- card gap: 16–24px

Do not create huge empty gaps that force excessive scrolling.

## Cards

Default:
- radius: 18–22px
- padding: 22–30px
- border: subtle plum/lavender, ~10% opacity
- shadow: broad, low-contrast

Dense report:
- reduce padding before reducing font size

## Hero

Use:
- large clear headline
- one concise supporting paragraph
- optional eyebrow
- one gradient or blurred atmospheric glow
- 1–3 important metrics if relevant

Avoid:
- overloaded hero cards
- multiple decorative shapes competing with content
- giant empty cover screens for operational reports

## Grid behavior

Use CSS Grid where possible.

Desktop:
- 2–4 columns depending on content density

Tablet:
- reduce columns based on minimum card width

Mobile:
- collapse logically to one column
- two compact metric cards may remain 2-column if legible

## Mobile

At <= 768px:
- page padding: 18–20px
- card padding: 18–20px
- h1 should usually stay <= 42px
- avoid fixed widths
- avoid horizontal overflow
- tables may scroll horizontally when conversion to cards would harm scanability

## Long reports

For >2 major sections:
- use sticky or compact TOC if helpful
- section anchors should be predictable
- use progressive detail
- do not flatten all detail into one continuous wall

## Density rule

For work reports:
- prefer compact cards
- use color only where it improves scanning
- do not decorate every section equally
