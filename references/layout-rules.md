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


## Presentation / PPT mode

When HTML is intended to be used like a PPT, presentation, pitch deck, internal review, or slide-style report, use this mode by default.

### Canvas

Canonical presentation canvas:
- aspect ratio: **16:9**
- working size: **1920×1080px**
- one HTML slide should map cleanly to one presentation frame
- no vertical scrolling inside a slide
- preserve generous edge margins and safe areas for projection / screen sharing

For browser preview, scale the 1920×1080 canvas responsively while preserving aspect ratio.

### Slide logic

Each slide should:
- communicate one dominant idea
- use a strong assertion-style headline when appropriate
- keep content density closer to PPT than dashboard/webpage density
- use whitespace intentionally
- avoid unrelated card grids when a simpler visual narrative works
- avoid turning the slide into a generic website hero with detached decoration

### Character integration

The canonical main girl is not a bottom-corner ornament.

Use her as part of the composition:
- leaning on or touching large type
- pointing to a key number, chart, or label
- standing on a baseline or beside a process step
- bridging headline and evidence
- anchoring a conclusion or transition

The role should have a clear visual reason to exist on the slide.

Supporting characters, especially the small dog, may:
- close negative space
- anchor the bottom of a type block
- support warm / playful / seasonal moments
- reinforce a transition or conclusion

Avoid:
- large character panel on the right with no relationship to the message
- character dropped into the bottom-right only as decoration
- multiple large characters competing on one slide
- decorative stickers that do not support hierarchy or narrative

### Default slide composition

A strong default cover / title composition may use:
- small eyebrow / context label at top left
- page number or section marker at top right
- oversized stacked headline occupying 45–60% of the frame
- canonical line-art girl physically interacting with the headline
- small dog near the baseline as a secondary anchor
- one short supporting sentence below or beside the title
- no more than 1–3 tiny doodle accents

This is a starting pattern, not a mandatory template.
