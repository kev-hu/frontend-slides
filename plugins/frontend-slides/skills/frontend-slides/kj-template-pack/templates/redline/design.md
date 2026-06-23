---
version: alpha
name: Redline
description: "A Swiss/International-style presentation system on pure white with a single hot-red (#ff3300) carrying every accent. Display runs Archivo Black (900) — oversized, tightly tracked, near-lowercase headlines that dominate the slide; body runs Nunito; all labels, eyebrows, citations and the page counter run JetBrains Mono in uppercase with wide tracking. The signature move is restraint plus one loud commitment: a thin Swiss hairline grid behind everything, hard 2px black bordered boxes with zero rounded corners, numbered mono eyebrows (01 / LABEL), short fat red rule-bars, and a single red doing every emphasis — key phrases, numerals, the quote mark, the period after a statement. It reads as engineered, editorial, and high-contrast — Bauhaus poster meets technical spec sheet — and looks authoritative without going corporate-soft."

colors:
  paper: "#ffffff"
  ink: "#0a0a0a"
  gray: "#555555"
  gray-2: "#8a8a8a"
  red: "#ff3300"
  line: "#e9e7e2"

typography:
  kicker:
    fontFamily: "'JetBrains Mono', monospace"
    fontWeight: 700
    fontSize: "24px"
    lineHeight: 1.2
    letterSpacing: "0.22em"
    textTransform: "uppercase"
    color: "{colors.gray-2}"
  eyebrow:
    fontFamily: "'JetBrains Mono', monospace"
    fontWeight: 700
    fontSize: "26px"
    lineHeight: 1.2
    letterSpacing: "0.02em"
    textTransform: "uppercase"
    color: "{colors.ink}"
  hero-title:
    fontFamily: "'Archivo', sans-serif"
    fontWeight: 900
    fontSize: "168px"
    lineHeight: 0.86
    letterSpacing: "-0.045em"
    color: "{colors.ink}"
  statement:
    fontFamily: "'Archivo', sans-serif"
    fontWeight: 900
    fontSize: "116px"
    lineHeight: 0.95
    letterSpacing: "-0.04em"
    color: "{colors.ink}"
  title:
    fontFamily: "'Archivo', sans-serif"
    fontWeight: 900
    fontSize: "92px"
    lineHeight: 0.95
    letterSpacing: "-0.04em"
    color: "{colors.ink}"
  lead:
    fontFamily: "'Nunito', sans-serif"
    fontWeight: 500
    fontSize: "36px"
    lineHeight: 1.45
    color: "{colors.ink}"
  body:
    fontFamily: "'Nunito', sans-serif"
    fontWeight: 400
    fontSize: "26px"
    lineHeight: 1.5
    color: "{colors.gray}"
  stat-num:
    fontFamily: "'Archivo', sans-serif"
    fontWeight: 900
    fontSize: "76px"
    lineHeight: 1
    letterSpacing: "-0.03em"
    color: "{colors.ink}"
  stat-label:
    fontFamily: "'JetBrains Mono', monospace"
    fontWeight: 700
    fontSize: "19px"
    lineHeight: 1.2
    letterSpacing: "0.06em"
    textTransform: "uppercase"
    color: "{colors.gray}"
  card-num:
    fontFamily: "'Archivo', sans-serif"
    fontWeight: 900
    fontSize: "30px"
    lineHeight: 1
    color: "{colors.red}"
  card-title:
    fontFamily: "'Archivo', sans-serif"
    fontWeight: 800
    fontSize: "30px"
    lineHeight: 1.1
    letterSpacing: "-0.02em"
    color: "{colors.ink}"
  card-body:
    fontFamily: "'Nunito', sans-serif"
    fontWeight: 400
    fontSize: "23px"
    lineHeight: 1.45
    color: "{colors.gray}"
  bigstat-num:
    fontFamily: "'Archivo', sans-serif"
    fontWeight: 900
    fontSize: "104px"
    lineHeight: 1
    letterSpacing: "-0.04em"
    color: "{colors.red}"
  bigstat-label:
    fontFamily: "'Nunito', sans-serif"
    fontWeight: 600
    fontSize: "24px"
    lineHeight: 1.2
    color: "{colors.ink}"
  bigstat-desc:
    fontFamily: "'Nunito', sans-serif"
    fontWeight: 400
    fontSize: "20px"
    lineHeight: 1.4
    color: "{colors.gray}"
  quote:
    fontFamily: "'Archivo', sans-serif"
    fontWeight: 800
    fontSize: "78px"
    lineHeight: 1.05
    letterSpacing: "-0.03em"
    color: "{colors.ink}"
  quote-mark:
    fontFamily: "'Archivo', sans-serif"
    fontWeight: 900
    fontSize: "240px"
    lineHeight: 0.4
    color: "{colors.red}"
  cite:
    fontFamily: "'JetBrains Mono', monospace"
    fontWeight: 700
    fontSize: "24px"
    lineHeight: 1.2
    letterSpacing: "0.08em"
    textTransform: "uppercase"
    color: "{colors.gray}"
  pointer-label:
    fontFamily: "'JetBrains Mono', monospace"
    fontWeight: 700
    fontSize: "26px"
    lineHeight: 1.2
    color: "{colors.red}"
  pointer-text:
    fontFamily: "'Nunito', sans-serif"
    fontWeight: 400
    fontSize: "24px"
    lineHeight: 1.4
    color: "{colors.gray}"
  counter:
    fontFamily: "'JetBrains Mono', monospace"
    fontWeight: 400
    fontSize: "20px"
    lineHeight: 1
    color: "{colors.gray}"

spacing:
  content-inset: "96px 130px 118px"
  gap-block: "34px"
  gap-cards: "26px"
  grid-line-x1: "130px"
  grid-line-x2: "960px"
  rule-bar-w: "120px"
  rule-bar-h: "12px"

canvas:
  width: 100vw
  height: 100vh
  background: "{colors.paper}"

components:
  rule-bar:
    width: "120px"
    height: "12px"
    background: "{colors.red}"
    description: "Short fat red bar, 120x12, hard corners. Sits above hero/section/closing titles as the only graphic punctuation. Never more than one per slide."
  eyebrow-number:
    fontFamily: "'JetBrains Mono', monospace"
    fontWeight: 700
    color: "{colors.red}"
    description: "The leading 'NN' of a 'NN / LABEL' mono eyebrow, colored red while the slash and label stay ink. The deck's section-numbering motif."
  bordered-card:
    background: "{colors.paper}"
    border: "2px solid {colors.ink}"
    borderRadius: "0"
    padding: "34px 34px 38px"
    description: "The universal content card: hard 2px black outline on white, zero radius. Holds a red card-num, an Archivo card-title, and Nunito card-body. Never tinted, never shadowed, never rounded."
  bigstat-band:
    border: "2px solid {colors.ink}"
    borderRadius: "0"
    description: "A single bordered band split into equal cells by 2px ink dividers (no outer gap). Each cell holds a giant red bigstat-num over an ink label and gray desc. The system's dashboard moment."
  quote-mark:
    color: "{colors.red}"
    description: "Oversized red Archivo opening quote glyph (240px, line-height 0.4) sitting directly above the quote. The quote body stays ink; only the mark and one key phrase are red."
  pointer-card:
    background: "{colors.paper}"
    border: "2px solid {colors.ink}"
    borderRadius: "0"
    padding: "30px 32px"
    description: "Closing-slide reference card: a mono red pointer-label over gray pointer-text, in a hard 2px box. Used in pairs on the closing surface."
  grid-hairlines:
    color: "{colors.line}"
    description: "Two 1px vertical hairlines at x=130px (left structure column) and x=960px (center spine) at ~70% opacity, behind all content. The quiet Swiss substructure; never thicker, never colored."
  progress-bar:
    height: "6px"
    background: "{colors.red}"
    description: "Solid red strip pinned to the bottom edge of the stage; width = (slideIndex+1)/total. The only persistent color element besides accents."
  counter:
    fontFamily: "'JetBrains Mono', monospace"
    color: "{colors.gray}"
    description: "Mono 'NN / NN' page counter at the bottom-right of the content area."
---

## Frontend Slides Fixed-Stage Policy

When this design system is used by the `frontend-slides` skill, generate the final deck as a **fixed 1920×1080 stage** that scales uniformly to the browser viewport. The deck should preserve a 16:9 slide canvas on every screen, including phones; it may letterbox or pillarbox, but it should not reflow slide content for mobile.

This policy has higher priority than any source-template responsive behavior described later in this file. If a later section says the original template is viewport-fluid, treat that as source history only, not as the target generation model for `frontend-slides`.

This policy applies even if values below use `100vw`, `100vh`, `vw`, `vh`, or `clamp()`. Treat those as design proportions to translate into 1920×1080 stage coordinates, not as live responsive rules in the generated deck.

Render each slide at 1920×1080, scale the whole stage with one transform, and verify rendered screenshots for both text overflow and panel overlap.

## Overview

**Redline** is a Swiss/International-style deck system built on a single committed bet: **pure white, near-black ink, and exactly one hot-red (`{colors.red}` — `#ff3300`) that carries every accent in the deck.** There is no secondary color, no tint palette, no gradient. The red appears on the rule-bar, the eyebrow number, key phrases inside the lead, every large numeral on a stat surface, the quote mark, and the period after a statement — and nowhere else. That discipline is the identity: the deck reads as engineered and editorial because the color does exactly one job, loudly.

The type system runs **three faces with non-overlapping roles**. **Archivo** at weight 900 is the display face — oversized, tightly tracked (`-0.04em` to `-0.045em`), near-lowercase headlines that occupy a third of the slide and butt right up against the content below them. **Nunito** is the body face — friendly, readable, used for the lead paragraph and all card/stat supporting copy, never for a headline. **JetBrains Mono** is the label face — every eyebrow, kicker, citation, stat label, pointer label, and the page counter is mono, uppercase, and widely tracked. The contrast between a screaming Archivo headline and a quiet mono eyebrow is the system's voice.

The color philosophy is **one accent, three neutrals**. `{colors.ink}` (`#0a0a0a`) carries all display and primary text; `{colors.gray}` (`#555555`) carries body and supporting copy; `{colors.gray-2}` (`#8a8a8a`) is reserved for the cover kicker only. The red is never used for a full headline (headlines are always ink) — it punctuates. This is the inverse of a "brand color everywhere" deck: the red is rationed so each appearance lands.

Depth is **structural, not soft**. There are no shadows anywhere. Elevation is created two ways: a thin Swiss hairline grid sitting behind everything (a left structure column at 130px and a center spine at 960px), and hard **2px solid black borders with zero radius** on every card, stat band, and pointer box. Nothing is tinted, nothing is rounded, nothing floats. The grid says "this was laid out"; the hard borders say "this is precise."

**Density is medium and rhythmic.** Most slides carry a mono eyebrow at the top, one Archivo headline, and a single content block (a 3-card grid, a 3-cell stat band, or a pointer pair) pushed to the lower half via `margin-top: auto`. Big type up top, structured data down low, generous white space between — the slide breathes while still feeling packed with intent. Statement and quote surfaces drop the content block entirely for one dominant typographic moment.

**Key Characteristics:**
- Pure white (`{colors.paper}`) canvas on every surface — never tinted, never dark.
- A single hot-red (`{colors.red}`) carries every accent; no second color exists.
- Archivo 900 display, oversized and tightly tracked, in ink — never red, never light.
- Nunito body and JetBrains Mono labels — three faces, one job each, no crossover.
- Numbered mono eyebrows in the `NN / LABEL` form, the `NN` in red.
- Short fat red rule-bar (120×12) as the only graphic punctuation above titles.
- Hard 2px black borders with zero corner radius on every card and band.
- A thin Swiss hairline grid (130px + 960px verticals) behind all content.
- Zero shadows — depth comes from borders and the grid, never elevation blur.
- Red is rationed: rule, eyebrow number, key phrase, numerals, quote mark, the period.

## Colors

### Palette

- **Paper** (`{colors.paper}` — `#ffffff`): The universal canvas. Every slide, every card, every band sits on pure white. Never tinted, never swapped for a dark surface — Redline is a light-only system.
- **Ink** (`{colors.ink}` — `#0a0a0a`): Near-black. Carries every Archivo headline, the eyebrow slash + label, card titles, stat labels, and all card/band borders. The default text and structure color.
- **Gray** (`{colors.gray}` — `#555555`): Body and supporting copy — the lead's muted variant, card bodies, stat descriptions, citations, the counter. Reads as clearly secondary to ink without disappearing.
- **Gray-2** (`{colors.gray-2}` — `#8a8a8a`): Reserved for the **cover kicker only** — the one place the system uses a lighter-than-body gray, to keep the cover's top label quiet beneath the hero.
- **Red** (`{colors.red}` — `#ff3300`): The single accent. Used for the rule-bar, the eyebrow number, key phrases inside a lead/closing line, every large numeral on a stat/big-stat surface, the quote mark, the accent period after a statement, and the progress bar. Never used for a full headline or for body text.
- **Line** (`{colors.line}` — `#e9e7e2`): The hairline grid color only. 1px verticals behind content at ~70% opacity. Never used as a border on cards (those are ink), never as text.

### Defaults

- **Default surface**: `{colors.paper}` — always pure white.
- **Default headline color**: `{colors.ink}` — Archivo display is always near-black. Red headlines are forbidden.
- **Default body color**: `{colors.gray}` for supporting copy; the lead paragraph may use `{colors.ink}` for its plain run with `{colors.red}` on the one phrase being emphasized.
- **Default label/eyebrow color**: `{colors.ink}` for the slash + label text, `{colors.red}` for the leading number.
- **Default border color**: `{colors.ink}` at 2px. Always. Card borders are never red, never gray, never hairline.
- **Default numeral color on a stat surface**: `{colors.red}` — big numbers are the accent moment.

The system has **no second accent color**. Do not introduce blue, green, or a tint of red to differentiate categories — distinguish through position, size, numbering, or label, never through an added hue.

## Typography

### Font Family Stack

Three Google Fonts, each with one role and no crossover.

**Archivo** (weights 800–900) is the display + numerical face: every hero, statement, section title, card title, stat numeral, and quote. Weight 900 for headlines and numerals, 800 for card titles and the quote body. Its grotesque, slightly condensed forms at heavy weight give the deck its blunt, engineered authority.

**Nunito** (weights 400–600) is the body face: the lead paragraph, card bodies, stat labels/descriptions, and pointer text. Its rounded humanist forms soften the otherwise hard system so it reads as confident, not cold.

**JetBrains Mono** (weights 400–700) is the label face: every eyebrow, kicker, citation, stat label, pointer label, and the page counter — always uppercase with wide tracking. The mono labels are the deck's "technical readout" voice against the screaming Archivo display.

### Typography Scale

| Token | Size | Family | Weight | Use |
|---|---|---|---|---|
| `{typography.hero-title}` | 168px | Archivo | 900 | Cover headline |
| `{typography.statement}` | 116px | Archivo | 900 | Section / statement headline |
| `{typography.title}` | 92px | Archivo | 900 | Content / stat / closing slide title |
| `{typography.quote}` | 78px | Archivo | 800 | Quote body |
| `{typography.quote-mark}` | 240px | Archivo | 900 | Oversized red opening quote glyph |
| `{typography.bigstat-num}` | 104px | Archivo | 900 | Giant numeral in a stat band cell (red) |
| `{typography.stat-num}` | 76px | Archivo | 900 | Cover stat-row numeral |
| `{typography.lead}` | 36px | Nunito | 500 | Lead paragraph under a headline |
| `{typography.card-title}` | 30px | Archivo | 800 | Bordered-card title |
| `{typography.card-num}` | 30px | Archivo | 900 | Bordered-card index number (red) |
| `{typography.eyebrow}` | 26px | JetBrains Mono | 700 | `NN / LABEL` section eyebrow |
| `{typography.pointer-label}` | 26px | JetBrains Mono | 700 | Closing pointer-card label (red) |
| `{typography.body}` | 26px | Nunito | 400 | General body / supporting paragraph |
| `{typography.bigstat-label}` | 24px | Nunito | 600 | Stat-band cell label |
| `{typography.kicker}` | 24px | JetBrains Mono | 700 | Cover top kicker (gray-2) |
| `{typography.cite}` | 24px | JetBrains Mono | 700 | Quote attribution |
| `{typography.pointer-text}` | 24px | Nunito | 400 | Closing pointer-card body |
| `{typography.card-body}` | 23px | Nunito | 400 | Bordered-card body |
| `{typography.counter}` | 20px | JetBrains Mono | 400 | Page counter |
| `{typography.bigstat-desc}` | 20px | Nunito | 400 | Stat-band cell description |
| `{typography.stat-label}` | 19px | JetBrains Mono | 700 | Cover stat-row label |

### Defaults

- **Cover headline**: `{typography.hero-title}` (168px). One short line; the biggest type in the deck.
- **Section / statement headline**: `{typography.statement}` (116px), often two lines with a red accent period.
- **Every other slide title**: `{typography.title}` (92px), single line.
- **Lead under a headline**: `{typography.lead}` (36px), max ~1180px wide, one red phrase.
- **Section eyebrow**: `{typography.eyebrow}` in the `NN / LABEL` form — reach for this on every content/section/closing slide.
- **Any large numeral**: `{typography.bigstat-num}` (band) or `{typography.stat-num}` (cover row), always red.

### Signature Treatments

These are non-optional whenever the element appears:

- **Every Archivo headline is ink, never red, with negative tracking (`-0.04em`/`-0.045em`).** The red never touches a full headline — it punctuates around it. Default-tracked Archivo reads as untreated.
- **Every eyebrow is `NN / LABEL` in JetBrains Mono uppercase, with the `NN` in red and the slash + label in ink.** This numbering motif is the deck's structural spine; an un-numbered eyebrow breaks the system.
- **Every title/section/closing headline is preceded by a single red rule-bar** (`{components.rule-bar}`, 120×12, hard corners). One per slide, never more.
- **Every large numeral is red Archivo 900.** Numbers are the accent moment; an ink numeral on a stat surface collapses the hierarchy.
- **Every card and band uses a hard 2px ink border with zero radius.** No tint, no shadow, no rounded corner — ever.
- **Labels are mono, body is Nunito, headlines are Archivo — never cross the faces.** A Nunito headline or an Archivo body run reads as a different deck.

## Layout

### Canvas System

Each slide is the fixed 1920×1080 stage. Content lives in a single `.content` block inset `{spacing.content-inset}` (96px top, 130px left/right, 118px bottom) — the left inset deliberately aligns the content edge to the left grid hairline at 130px. Blocks stack top-to-bottom with `{spacing.gap-block}` (34px) between them; the primary content block (grid/band/pointer pair) is pushed to the lower half with `margin-top: auto`, leaving the headline up top and white space between.

### Persistent Chrome

Two elements recur on every slide:
- **Progress bar** (`{components.progress-bar}`) — a 6px red strip pinned to the bottom edge, width = `(slideIndex+1)/total * 100%`.
- **Counter** (`{components.counter}`) — a mono `NN / NN` page counter at the bottom-right of the content area.

### Surface Variations

The deck cycles through six archetypes: **cover** (kicker + rule + hero + lead + 3-up stat row), **section** (eyebrow + rule + statement + lead, centered in the vertical spread), **content** (eyebrow + title + 3-card bordered grid), **stat** (eyebrow + title + 3-cell bordered stat band), **quote** (oversized red quote mark + Archivo quote + mono cite), and **closing** (eyebrow + rule + title + pointer-card pair + one red-accented closing line).

### The Hairline Grid

The signature composition device is the Swiss hairline grid (`{components.grid-hairlines}`): two 1px `{colors.line}` verticals at `{spacing.grid-line-x1}` (130px) and `{spacing.grid-line-x2}` (960px), behind all content at ~70% opacity. Content aligns to the left line; the center line marks the implied 2-column spine.

## Depth and Elevation

Redline uses **two structural depth mechanisms and zero shadows**:

1. **Hard 2px ink borders.** Cards, stat bands, and pointer boxes are defined entirely by a 2px `{colors.ink}` outline with no radius and no fill change. The border *is* the elevation — the box reads as a discrete unit because of its hard edge, not because it floats.
2. **The hairline grid.** The 1px substructure behind everything implies a coordinate system the content snaps to, which reads as "deliberately placed" — a quieter kind of depth than shadow.

There are **no `box-shadow` declarations anywhere** in the system, and no tinted surfaces. A shadow or a tinted card immediately reads as a different, softer aesthetic and breaks Redline's engineered character.

## Shapes and Treatment

### Border Radius

**Zero radius everywhere.** Every card, band, pointer box, rule-bar, and the progress bar has hard 90° corners. This is non-negotiable — a single rounded corner collapses the Swiss/brutalist register.

### Border Weight Ladder

- **2px solid `{colors.ink}`** — the universal card/band/pointer border, and the internal dividers of the stat band.
- **1px solid `{colors.line}`** — the hairline grid verticals only (decorative, behind content).

No other border weights exist. Borders are never red and never gray-on-card.

### Decorative Element Types

- **Rule-bar** (`{components.rule-bar}`) — 120×12 solid red block above titles. The deck's only purely graphic mark.
- **Eyebrow number** (`{components.eyebrow-number}`) — the red `NN` leading a mono `NN / LABEL` eyebrow.
- **Bordered card** (`{components.bordered-card}`) — hard 2px ink box, white fill, red index number, Archivo title, Nunito body.
- **Big-stat band** (`{components.bigstat-band}`) — one bordered band split by 2px ink dividers into equal cells, each with a giant red numeral.
- **Quote mark** (`{components.quote-mark}`) — oversized red Archivo opening-quote glyph above an ink quote.
- **Pointer card** (`{components.pointer-card}`) — closing reference box with a red mono label over gray text.
- **Grid hairlines** (`{components.grid-hairlines}`) — the 1px Swiss substructure.

## Do's and Don'ts

### Do

- Keep every surface on pure white `{colors.paper}`.
- Ration the red: rule-bar, eyebrow number, one key phrase, numerals, quote mark, the period — and nothing else.
- Set every headline in Archivo 900 ink with negative tracking; let the headline dominate the upper slide.
- Number every eyebrow `NN / LABEL` in JetBrains Mono, the `NN` in red.
- Put a single red rule-bar above hero/section/closing titles.
- Outline every card and band with a hard 2px ink border, zero radius.
- Make every large numeral red Archivo 900.
- Keep the three faces in their lanes: Archivo display, Nunito body, JetBrains Mono labels.
- Push the primary content block to the lower half and let the slide breathe above it.

### Don't

- Don't add a second accent color, or tint the red, to differentiate categories — use position, number, or label.
- Don't set a headline in red — headlines are always ink; red only punctuates.
- Don't round any corner, anywhere.
- Don't use shadows or tinted card fills — depth is borders + grid only.
- Don't make card borders red or gray — borders are 2px ink.
- Don't cross the type faces (no Nunito headline, no Archivo body, no sans label).
- Don't thicken or color the hairline grid — it stays 1px `{colors.line}`.
- Don't crowd the headline against the content block — the upper white space is part of the composition.

## Responsive Behavior

Redline is authored as a fixed **1920×1080** stage; all sizes above are stage pixels. The original reference uses one transform to scale the whole stage to the viewport (letterbox/pillarbox), never reflowing content. Under the `frontend-slides` skill the deck is rendered fixed-stage regardless — translate any proportional values into 1920×1080 coordinates and do not introduce mobile breakpoints that rearrange slide content. There is no separate small-screen layout; the stage simply scales down as a whole.

## CJK & International Content

The Swiss/grotesque structure transfers cleanly to CJK; only the type stack changes.

### Recommended Pairing

| Role | Latin (default) | CJK counterpart |
|---|---|---|
| Display / headline / numerals (Archivo 900) | Archivo 800–900 | 思源黑体 Noto Sans SC 900 |
| Body / lead / card body (Nunito) | Nunito 400–600 | 思源黑体 Noto Sans SC 400 |
| Labels / eyebrow / cite (JetBrains Mono) | JetBrains Mono 700 uppercase | 思源黑体 Noto Sans SC 500 (no transform) |

### Mixed-Content Strategy

Use one CJK family (思源黑体 Noto Sans SC) across all three roles, leaning on weight (900 / 500 / 400) to recover the Archivo-vs-mono contrast that CJK can't get from face-switching. Keep numerals in Latin Archivo where possible — large red Arabic numerals are the accent moment and read well in a CJK deck.

### Universal CJK Adjustments

- **Line-height**: raise display to ~1.1–1.2 and body to ~1.7; CJK glyphs crowd vertically.
- **Letter-spacing**: set to 0 on every CJK run — the `-0.04em` display tracking and the `0.22em` mono tracking both break CJK.
- **Text-transform**: remove `uppercase` on CJK (no case); keep the red `NN` number and the rule-bar to carry the eyebrow's chrome recognition instead.
- **Punctuation**: use full-width CJK punctuation; drop the trailing period on display headlines.
- **盘古之白**: insert a space between CJK and adjacent Latin/digits.

## Iteration Guide

1. Any new slide starts on `{colors.paper}` white with the hairline grid behind it.
2. A new content slide opens with a `NN / LABEL` mono eyebrow (red `NN`) and an Archivo 900 ink title.
3. A new section/statement slide gets a red rule-bar above a `{typography.statement}` headline, optionally with a red accent period.
4. A new list of 3 items → three `{components.bordered-card}` boxes with red index numbers; never a bullet list.
5. A new set of metrics → a `{components.bigstat-band}`, numerals in red `{typography.bigstat-num}`.
6. A new pull-quote → `{components.quote-mark}` in red above an ink `{typography.quote}` with a mono `{typography.cite}`.
7. A new emphasis inside body text → wrap the single key phrase in `{colors.red}`; never more than one per block.
8. A new closing → red rule-bar, `{typography.title}`, a pair of `{components.pointer-card}`, and one red-accented closing line.
9. Keep the primary content block pushed to the lower half (`margin-top: auto`); never fill the upper white space with decoration.
10. If a slide feels empty, enlarge the headline or add a stat band — never add a second color or a shadow.

## Known Gaps

- **Light-only.** There is no dark surface in the system; a dark slide would need a separate inverse spec.
- **Single display weight in practice.** Archivo is used almost entirely at 900 (800 only on the quote/card titles); the system's character depends on the heavy weight loading.
- **Google-Fonts dependent.** Archivo, Nunito, and JetBrains Mono load from Google Fonts with only generic fallbacks; if the CDN fails the deck collapses to system fonts and loses its identity.
- **Headlines must stay short.** The oversized Archivo display (92–168px) only fits 1–3 words per line at 1920 wide; long titles will wrap past their budget and must be shortened, not shrunk.
- **Single-accent limits categorical color.** Multi-series data can't be color-coded — distinguish by position, numbering, or label only. This is intentional but real.
- **The accent period** (a red `.` after a statement) renders as a chunky square at Archivo 900; treat it as a deliberate accent dot, and drop it for CJK.
