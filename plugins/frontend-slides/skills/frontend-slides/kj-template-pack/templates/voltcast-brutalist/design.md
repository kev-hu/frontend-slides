---
version: alpha
name: Voltcast
description: "A high-voltage brutalist hardware-spec system — acid-green-on-void, built like a synth front panel. The display face is Archivo Black, a single-weight ultra-heavy grotesque set in screaming uppercase at poster scale (96-360px) with tight negative tracking (-2px to -10px) and no rotation; the system's authority comes from sheer mass, not movement. Body and every label run JetBrains Mono — the body face for paragraphs and quote text, and the metadata voice for wide-tracked uppercase labels that always open with a // prefix, like a code comment. The palette is uncompromising single-accent: near-black void (#0B0B0F), one saturated acid green (#C6FF00), off-white bone (#EDEDE6) for primary text, muted gray (#8A8A82) for secondary body, and a dark wire gray (#2A2A33) for hairline grid rules. There are zero rounded corners, zero drop shadows, and zero gradients. Depth is purely structural: a 3px acid top-bar and 6px acid bottom progress-rule frame every slide, hard wire-thin grid rules separate cells (3px outer + 1px inner), and the one big move is surface inversion — a full-bleed acid panel flips the entire surface to void-on-acid for the stat moment. The register is loud, technical, and Berlin-industrial — closer to a Eurorack module's silkscreen than a corporate deck."

colors:
  void: "#0B0B0F"
  acid: "#C6FF00"
  bone: "#EDEDE6"
  muted: "#8A8A82"
  wire: "#2A2A33"

typography:
  hero-title:
    fontFamily: "'Archivo Black', sans-serif"
    fontWeight: 400
    fontSize: "clamp(72px, 11.5vw, 168px)"
    lineHeight: 0.86
    letterSpacing: "-2px"
    textTransform: "uppercase"
    color: "{colors.bone}"
  close-title:
    fontFamily: "'Archivo Black', sans-serif"
    fontWeight: 400
    fontSize: "clamp(64px, 10vw, 150px)"
    lineHeight: 0.86
    letterSpacing: "-2px"
    textTransform: "uppercase"
    color: "{colors.bone}"
  section-title:
    fontFamily: "'Archivo Black', sans-serif"
    fontWeight: 400
    fontSize: "clamp(48px, 6.5vw, 96px)"
    lineHeight: 0.86
    letterSpacing: "-2px"
    textTransform: "uppercase"
    color: "{colors.bone}"
  content-title:
    fontFamily: "'Archivo Black', sans-serif"
    fontWeight: 400
    fontSize: "clamp(36px, 4vw, 58px)"
    lineHeight: 0.9
    letterSpacing: "-1.5px"
    textTransform: "uppercase"
    color: "{colors.bone}"
  stat-figure:
    fontFamily: "'Archivo Black', sans-serif"
    fontWeight: 400
    fontSize: "clamp(160px, 25vw, 360px)"
    lineHeight: 0.78
    letterSpacing: "-10px"
    color: "{colors.void}"
  stat-unit:
    fontFamily: "'Archivo Black', sans-serif"
    fontWeight: 400
    fontSize: "clamp(56px, 8vw, 120px)"
    letterSpacing: "-4px"
    color: "{colors.void}"
  section-index:
    fontFamily: "'Archivo Black', sans-serif"
    fontWeight: 400
    fontSize: "clamp(140px, 15vw, 220px)"
    lineHeight: 0.8
    letterSpacing: "-6px"
    color: "{colors.wire}"
  cell-number:
    fontFamily: "'Archivo Black', sans-serif"
    fontWeight: 400
    fontSize: "clamp(40px, 3.5vw, 52px)"
    letterSpacing: "-1px"
    color: "{colors.acid}"
  spec-value:
    fontFamily: "'Archivo Black', sans-serif"
    fontWeight: 400
    fontSize: "clamp(22px, 2vw, 30px)"
    letterSpacing: "-1px"
    color: "{colors.bone}"
  brandmark:
    fontFamily: "'Archivo Black', sans-serif"
    fontWeight: 400
    fontSize: "22px"
    letterSpacing: "-1px"
    color: "{colors.acid}"
  quote-body:
    fontFamily: "'JetBrains Mono', monospace"
    fontWeight: 700
    fontSize: "clamp(36px, 4vw, 56px)"
    lineHeight: 1.28
    letterSpacing: "-1px"
    color: "{colors.bone}"
  body:
    fontFamily: "'JetBrains Mono', monospace"
    fontWeight: 400
    fontSize: "clamp(14px, 1.1vw, 17px)"
    lineHeight: 1.75
    color: "{colors.muted}"
  cell-body:
    fontFamily: "'JetBrains Mono', monospace"
    fontWeight: 400
    fontSize: "clamp(13px, 1vw, 15px)"
    lineHeight: 1.7
    color: "{colors.muted}"
  eyebrow:
    fontFamily: "'JetBrains Mono', monospace"
    fontWeight: 700
    fontSize: "15px"
    letterSpacing: "4px"
    textTransform: "uppercase"
    color: "{colors.acid}"
  label:
    fontFamily: "'JetBrains Mono', monospace"
    fontWeight: 700
    fontSize: "13px"
    letterSpacing: "3px"
    textTransform: "uppercase"
    color: "{colors.bone}"
  cell-label:
    fontFamily: "'JetBrains Mono', monospace"
    fontWeight: 700
    fontSize: "21px"
    letterSpacing: "2px"
    textTransform: "uppercase"
    color: "{colors.bone}"
  stat-caption:
    fontFamily: "'JetBrains Mono', monospace"
    fontWeight: 700
    fontSize: "clamp(18px, 1.6vw, 22px)"
    letterSpacing: "3px"
    textTransform: "uppercase"
    color: "{colors.void}"
  cite-name:
    fontFamily: "'JetBrains Mono', monospace"
    fontWeight: 700
    fontSize: "17px"
    letterSpacing: "2px"
    textTransform: "uppercase"
    color: "{colors.bone}"
  cite-role:
    fontFamily: "'JetBrains Mono', monospace"
    fontWeight: 400
    fontSize: "14px"
    letterSpacing: "1px"
    color: "{colors.muted}"
  spec-key:
    fontFamily: "'JetBrains Mono', monospace"
    fontWeight: 700
    fontSize: "11px"
    letterSpacing: "3px"
    textTransform: "uppercase"
    color: "{colors.muted}"
  cta:
    fontFamily: "'JetBrains Mono', monospace"
    fontWeight: 700
    fontSize: "16px"
    letterSpacing: "3px"
    textTransform: "uppercase"
    color: "{colors.void}"
  counter:
    fontFamily: "'JetBrains Mono', monospace"
    fontWeight: 700
    fontSize: "12px"
    letterSpacing: "3px"
    textTransform: "uppercase"
    color: "{colors.muted}"

spacing:
  pad-slide: "72px 96px"
  pad-cell: "34px 32px 38px"
  gap-spec: "0px"
  max-width-body: "760px"
  max-width-quote: "1500px"

canvas:
  width: 100vw
  height: 100vh
  background: "{colors.void}"

components:
  topbar:
    position: "absolute, top 0 left 0 right 0"
    borderTop: "3px solid {colors.acid}"
    description: "Persistent 3px acid rule pinned to the top edge of every slide. On the acid stat panel it inverts to a 3px void rule. The deck's upper frame element — reads as a circuit-board silkscreen trim."
  foot-rule:
    position: "absolute, bottom 0 left 0"
    height: "6px"
    background: "{colors.acid}"
    description: "Persistent 6px acid progress rule on the bottom edge. Its width grows with slide index (38% -> 100% across the deck), doubling as a progress bar and the lower poster-trim. Inverts to void on the acid stat panel."
  brandmark:
    position: "absolute, top 30px left 96px"
    fontFamily: "'Archivo Black', sans-serif"
    color: "{colors.acid}"
    description: "Persistent top-left wordmark in Archivo Black acid at 22px. The only place Archivo Black appears at small size. Inverts to void on the acid stat panel."
  slug:
    position: "absolute, top 36px right 96px"
    color: "{colors.muted}"
    description: "Persistent top-right context slug in JetBrains Mono 700 uppercase, always opening with a // prefix (e.g. // SPEC SHEET). The 'breadcrumb' chrome voice."
  counter:
    position: "absolute, bottom 30px right 96px"
    color: "{colors.muted}"
    description: "Persistent NN / NN slide counter in JetBrains Mono 700 uppercase, 3px tracking, muted gray. Bottom-right."
  mono-eyebrow:
    fontFamily: "'JetBrains Mono', monospace"
    fontWeight: 700
    color: "{colors.acid}"
    glyphPrefix: "//"
    description: "The system's universal section opener: acid JetBrains Mono 700 uppercase at 15px / 4px tracking, always prefixed with '// '. Used above every hero, section title, content title, stat figure, and closing title. The // prefix is the single most repeated micro-signature."
  wire-grid:
    borderTop: "3px solid {colors.wire}"
    borderLeft: "3px solid {colors.wire}"
    description: "The content-grid container: a 3px wire outer border on top+left, with each cell carrying 1px wire right+bottom borders. The 3px-outer / 1px-inner weight pair produces a hard tabular grid that reads as a panel layout silkscreen. No rounded corners, ever."
  grid-cell:
    borderRight: "1px solid {colors.wire}"
    borderBottom: "1px solid {colors.wire}"
    padding: "34px 32px 38px"
    minHeight: "300px"
    description: "A single content cell inside the wire-grid. Holds an Archivo Black acid number, a JetBrains Mono 700 uppercase title, and a JetBrains Mono 400 muted body paragraph. 1px wire borders only — the heavy 3px lives on the parent container."
  spec-row:
    borderTop: "1px solid {colors.wire}"
    display: "flex"
    description: "The cover's bottom metadata strip: a flex row of 3 specs divided by 1px wire vertical rules, each spec a tiny mono spec-key over an Archivo Black bone spec-value. The cover's data signature."
  acid-panel:
    background: "{colors.acid}"
    color: "{colors.void}"
    description: "Full-bleed acid-green surface inversion — the deck's one big move. The entire slide flips to void-on-acid; the stat figure becomes void Archivo Black on acid, chrome (topbar, foot-rule, brandmark, slug, counter) all invert to void. Used for the stat / statement moment only."
  acid-leftbar-cite:
    borderLeft: "4px solid {colors.acid}"
    paddingLeft: "22px"
    description: "Citation block under a quote, marked only by a 4px acid left rule + 22px padding-left. Holds a JetBrains Mono 700 uppercase name over a JetBrains Mono 400 muted role line. The system's only leftbar pattern — cantilevered off the acid rule, no enclosing box."
  acid-cta:
    background: "{colors.acid}"
    color: "{colors.void}"
    padding: "20px 36px"
    description: "Closing-slide call-to-action: a hard-edged solid acid block with void JetBrains Mono 700 uppercase text and a trailing arrow glyph. Zero border-radius. The one filled acid button in the system."
  acid-emphasis:
    color: "{colors.acid}"
    description: "Inline word-level emphasis: a single word inside a bone display title or mono quote switched to acid color. The only emphasis mechanism — never bold-on-bold, never underline, just the acid color swap on one word."
---

## Frontend Slides Fixed-Stage Policy

When this design system is used by the `frontend-slides` skill, generate the final deck as a **fixed 1920×1080 stage** that scales uniformly to the browser viewport. The deck should preserve a 16:9 slide canvas on every screen, including phones; it may letterbox or pillarbox, but it should not reflow slide content for mobile.

This policy has higher priority than any source-template responsive behavior described later in this file. If a later section says the original template is viewport-fluid, treat that as source history only, not as the target generation model for `frontend-slides`.

This policy applies even if values below use `100vw`, `100vh`, `vw`, `vh`, or `clamp()`. Treat those as design proportions to translate into 1920×1080 stage coordinates, not as live responsive rules in the generated deck.

Render each slide at 1920×1080, scale the whole stage with one transform, and verify rendered screenshots for both text overflow and panel overlap.

## Overview

Voltcast is a **high-voltage brutalist hardware-spec system** that lifts its vocabulary from synthesizer front panels, Eurorack module silkscreens, and Berlin-industrial product pages. The premise is that every slide should read like the face of a piece of analog hardware: screaming uppercase display set in pure mass, code-comment metadata labels, hard grid rules instead of cards, and exactly one electric accent burning against a near-black void. The system's authority is voltage, not polish — it gets louder, never softer.

The type system is **two faces in three roles**. **Archivo Black** (Google Fonts, single weight 400) is the display face — an ultra-heavy grotesque with closed apertures and slab-square terminals. It carries every hero title, section title, content title, stat figure, section index, and cell number. It is always uppercase, always tightly tracked (-1px to -10px depending on scale), and — unlike most poster systems — **never rotated**. The character work is sheer black mass at scale (96-360px); tilt would dilute it. **JetBrains Mono** (Google Fonts, weights 400 / 700) plays two roles at once: the **body voice** (weight 400, muted gray, 1.7-1.75 line-height, paragraphs and quote text in weight 700) and the **metadata voice** (weight 700, uppercase, 3-4px tracking — every label, eyebrow, spec key, cite, counter, and CTA). The monospace grid gives the whole system a technical, instrument-readout register that a proportional sans could not.

The single most repeated micro-signature is the **`// ` prefix** on every eyebrow and slug — labels open like code comments (`// SPEC SHEET`, `// HEADROOM`). It is the system's verbal tic and appears on every slide.

The color philosophy is **uncompromising single-accent**: near-black void (`{colors.void}` — `#0B0B0F`), one saturated acid green (`{colors.acid}` — `#C6FF00`), off-white bone (`{colors.bone}` — `#EDEDE6`) for primary display text, muted gray (`{colors.muted}` — `#8A8A82`) for secondary body, and dark wire gray (`{colors.wire}` — `#2A2A33`) for hairline grid rules and the ghosted section index. There are no secondary brand colors, no gradients, no tints, no semantic state colors. Acid is reserved for emphasis moments — eyebrows, the brandmark, cell numbers, one emphasis word per title, the leftbar rule, the CTA, and the persistent top/bottom rules — and is never used as body text or as a card fill that isn't either the full-bleed inversion panel or the CTA button.

Depth is **structural and flat — there are zero box-shadows and zero gradients in the entire system.** Depth comes from three mechanisms only: (1) the hard **wire grid** (3px outer + 1px inner border weights touching at cell intersections), (2) **surface inversion** (the full-bleed acid panel flips void↔acid for the stat moment), and (3) **scale contrast** (a 360px stat figure or a 220px ghosted section index against tiny 11-15px mono metadata). The system picks the "borders + inversion + scale" lane and commits; it never reaches for shadow or tilt.

**Density philosophy: medium-high — technical and packed, but ordered.** Content slides carry a full 3-cell wire grid with numbers, titles, and body paragraphs and read as a spec sheet, not a crowd. Hero, stat, quote, and closing slides intentionally drop to one or two huge display elements with large negative space — the polarities are deliberate. The cover sits in between: a 3-line display stack plus a 3-spec footer strip.

**Key Characteristics:**
- Near-black void (`{colors.void}`) canvas on every slide except the one full-bleed acid (`{colors.acid}`) stat-inversion panel.
- Single acid green (`{colors.acid}`) accent — eyebrows, brandmark, cell numbers, one emphasis word per title, leftbar rule, CTA, and the persistent top/bottom rules. Nothing else is colored.
- Two-face stack: Archivo Black (all uppercase display + numerals) and JetBrains Mono (body in 400 + every label/eyebrow/cite/counter in 700).
- The `// ` code-comment prefix on every eyebrow and slug — the system's verbal signature.
- Display Archivo Black is set in screaming uppercase at 96-360px with tight negative tracking and **never rotated** — mass is the move, not tilt.
- Persistent acid chrome frame: a 3px acid top-bar and a 6px acid bottom progress-rule (growing with slide index) on every slide.
- Hard wire grids: 3px outer + 1px inner border weights, zero rounded corners anywhere.
- Surface inversion (full-bleed acid panel, void text + inverted chrome) as the one statement move.
- Inline emphasis is a single-word acid color swap — never bold, never underline.
- The acid leftbar cite (4px acid rule + padding-left) and the solid acid CTA block are the only two filled/ruled acid components.

## Colors

### Palette

- **Void** (`{colors.void}` — `#0B0B0F`): Near-black with a faint blue bias, not pure black. The default canvas on every slide. Also the text color on the inverted acid panel (stat figure, caption, chrome) and inside the acid CTA. Reads as a powered-off panel.
- **Acid** (`{colors.acid}` — `#C6FF00`): Saturated acid/lime green — the system's single accent and its highest-voltage element. Used for every eyebrow, the brandmark, every cell number, one emphasis word per display title, the quote open-mark, the leftbar cite rule, the CTA fill, and the persistent top (3px) and bottom (6px) rules. As a surface it appears only as the full-bleed stat-inversion panel. Never used as body text, never as a card fill outside the inversion panel and the CTA, never tinted.
- **Bone** (`{colors.bone}` — `#EDEDE6`): Warm off-white. The default color for primary display text (hero, section, content, close titles), the non-acid words in those titles, the spec values, the cell titles, the quote body, and the cite name. The system's "ink." Never pure white.
- **Muted** (`{colors.muted}` — `#8A8A82`): Desaturated warm gray. Used for all secondary body — paragraphs, cell body, spec keys, slug, cite role, and the counter. The readable-but-recessive voice that keeps acid and bone dominant.
- **Wire** (`{colors.wire}` — `#2A2A33`): Dark cool gray, just above void. Used only for structural lines — the grid borders (3px outer, 1px inner), the cover spec-row dividers, and the giant ghosted section index numeral. Never used for text meant to be read.

### Defaults

- **Default surface background**: `{colors.void}`. For the statement moment, switch the whole surface to `{colors.acid}` (the inversion panel) — this is the only non-void surface.
- **Default display / headline color**: `{colors.bone}` on void surfaces; `{colors.void}` on the acid panel.
- **Default emphasis color inside a headline**: `{colors.acid}` on exactly one word.
- **Default body text color**: `{colors.muted}` on void surfaces; `{colors.void}` on the acid panel.
- **Default eyebrow / label color**: `{colors.acid}` for eyebrows (with the `// ` prefix); `{colors.muted}` for the slug and counter; `{colors.bone}` for cell titles and cite names; `{colors.void}` for all labels on the acid panel.
- **Default numeral color**: `{colors.acid}` for cell numbers; `{colors.wire}` for the ghosted section index; `{colors.void}` for the inverted stat figure.
- **Default border color**: `{colors.wire}`. There are no acid or bone borders except the 4px acid leftbar cite rule and the 3px/6px acid edge rules.
- **Default accent-rule color**: `{colors.acid}` (topbar, foot-rule, leftbar cite, section-title underline rule).

The system commits **hard** to the five-token palette and is functionally a **two-color identity** (void + acid) with bone/muted/wire as neutral support. Don't add a sixth color, and don't add a second accent (no red for warning, no blue for info). All categorical difference comes from position, number, label, and the void↔acid inversion — never from a new hue.

## Typography

### Font Family Stack

The system runs **two faces** across three roles.

**Archivo Black** (Google Fonts, single weight 400) is the display + numeral face — an ultra-heavy grotesque with closed apertures, slab-square terminals, and almost no internal counter space. It carries every hero title, section title, content title, section index, stat figure, cell number, spec value, and the brandmark. Always uppercase, always tightly tracked (-1px at small sizes down to -10px on the 360px stat figure), and **never rotated**. The face has no other weights; all hierarchy comes from size and color.

**JetBrains Mono** (Google Fonts, weights 400 + 700) is both the body face and the metadata face. As **body** (weight 400): paragraphs, cell body, spec keys, slug, cite role, and counter — set in `{colors.muted}` at 1.7-1.75 line-height. As **quote body** it steps up to weight 700 in `{colors.bone}`. As **metadata** (weight 700, uppercase, 3-4px tracking): every eyebrow, label, cell title, cite name, stat caption, and CTA. The monospace forms give the system its instrument-readout register.

The roles are non-overlapping: Archivo Black owns every display and numerical moment; JetBrains Mono owns every paragraph, quote, label, and chrome element. Don't cross them — Archivo Black body would be an unreadable black wall, and JetBrains Mono headlines would lose the mass that defines the system.

### Typography Scale

| Token | Size (clamp / px) | Family | Weight | Use |
|---|---|---|---|---|
| `{typography.stat-figure}` | 160–360px clamp | Archivo Black | 400 | Hero-class stat numeral (void, on acid panel) |
| `{typography.section-index}` | 140–220px clamp | Archivo Black | 400 | Ghosted wire section number behind a section title |
| `{typography.hero-title}` | 72–168px clamp | Archivo Black | 400 | Cover title (multi-line uppercase stack, one acid word) |
| `{typography.close-title}` | 64–150px clamp | Archivo Black | 400 | Closing-slide title (one acid word) |
| `{typography.stat-unit}` | 56–120px clamp | Archivo Black | 400 | Unit glyph trailing the stat figure (e.g. V) |
| `{typography.section-title}` | 48–96px clamp | Archivo Black | 400 | Section-header title (one acid word) |
| `{typography.content-title}` | 36–58px clamp | Archivo Black | 400 | Content-slide title above a grid |
| `{typography.quote-body}` | 36–56px clamp | JetBrains Mono | 700 | Quote text (bone, one acid emphasis word) |
| `{typography.cell-number}` | 40–52px clamp | Archivo Black | 400 | Wire-grid cell numeral (always acid) |
| `{typography.spec-value}` | 22–30px clamp | Archivo Black | 400 | Cover spec-row value (bone) |
| `{typography.brandmark}` | 22px | Archivo Black | 400 | Persistent top-left wordmark (acid) |
| `{typography.cell-label}` | 21px | JetBrains Mono | 700 | Wire-grid cell title (uppercase, 2px tracking) |
| `{typography.stat-caption}` | 18–22px clamp | JetBrains Mono | 700 | Caption under the stat figure (void, uppercase) |
| `{typography.cite-name}` | 17px | JetBrains Mono | 700 | Quote attribution name (uppercase) |
| `{typography.body}` | 14–17px clamp | JetBrains Mono | 400 | Standard body paragraph (muted) |
| `{typography.eyebrow}` | 15px | JetBrains Mono | 700 | `// ` section eyebrow (acid, 4px tracking) |
| `{typography.cell-body}` | 13–15px clamp | JetBrains Mono | 400 | Wire-grid cell body paragraph (muted) |
| `{typography.cite-role}` | 14px | JetBrains Mono | 400 | Quote attribution role line (muted) |
| `{typography.label}` | 13px | JetBrains Mono | 700 | Generic uppercase label (bone, 3px tracking) |
| `{typography.counter}` | 12px | JetBrains Mono | 700 | Persistent slide counter + top-right `// ` slug (muted, 3px tracking) |
| `{typography.spec-key}` | 11px | JetBrains Mono | 700 | Cover spec-row key (muted, 3px tracking) |
| `{typography.cta}` | 16px | JetBrains Mono | 700 | Closing CTA text (void on acid, 3px tracking) |

### Defaults

- **Default cover/hero title**: `{typography.hero-title}` (72–168px) as a multi-line uppercase Archivo Black stack with exactly one line or word in `{colors.acid}`.
- **Default section header**: `{typography.section-title}` (48–96px), preceded by a `{typography.section-index}` ghost numeral in `{colors.wire}` and a `// ` `{typography.eyebrow}`.
- **Default content-slide title**: `{typography.content-title}` (36–58px), with a `// ` eyebrow above and a wire grid below.
- **Default hero-class statistic**: `{typography.stat-figure}` (160–360px) in `{colors.void}` on a full-bleed `{colors.acid}` panel, with a `{typography.stat-unit}` glyph trailing if there's a unit.
- **Default wire-cell numeral**: `{typography.cell-number}` (40–52px) in `{colors.acid}`.
- **Default body**: `{typography.body}` (14–17px) JetBrains Mono 400 in `{colors.muted}` at line-height 1.75.
- **Default eyebrow**: `{typography.eyebrow}` (15px) JetBrains Mono 700 acid uppercase, 4px tracking, always prefixed with `// `.
- **Default weight for Archivo Black**: 400 — the only weight available.
- **Default weight for JetBrains Mono labels**: 700; body and cite-role drop to 400.

When unsure which display token to reach for, default to `{typography.section-title}` (48–96px) for a primary slide opener; reserve `{typography.stat-figure}` for the single stat-inversion moment and `{typography.hero-title}` for cover-class surfaces.

### Signature Treatments

These treatments are **non-optional whenever the corresponding element type is used**:

- **Every eyebrow and every slug opens with `// `.** The code-comment prefix is the system's verbal signature; an eyebrow without it is not the system's eyebrow.
- **Every display title carries exactly one `{colors.acid}` word or line; the rest is `{colors.bone}`.** Single-word acid emphasis is the only emphasis mechanism — no bold, no underline, no second accent.
- **Display Archivo Black is never rotated.** Mass at scale (with tight negative tracking) is the system's authority; tilt dilutes the front-panel weight. (This is the deliberate inverse of a tilt-based poster system.)
- **The stat moment is always a full-bleed `{colors.acid}` inversion panel** with a void Archivo Black figure, void caption, and all chrome (topbar, foot-rule, brandmark, slug, counter) inverted to void. A stat on the void surface is not the system's stat.
- **Every section header is preceded by a giant ghosted `{colors.wire}` section-index numeral** at 140–220px. The ghost numeral is the section archetype's structural signature.
- **Every quote uses an acid Archivo Black open-quote mark above a JetBrains Mono 700 body**, with the attribution in an `{components.acid-leftbar-cite}` (4px acid left rule).
- **Every content grid uses the wire double-weight border** (3px outer + 1px inner). Cells never get individual full outlines; the grid is one continuous ruled panel.
- **Every numeral that labels a cell is acid Archivo Black.** Cell numerals in bone or muted break the hierarchy — acid is the count signal.

### Typography Principles

The voice contrast is **screaming uppercase Archivo Black mass ↔ technical JetBrains Mono readout**. There is no serif, no italic, and no rotation anywhere in the system. Emphasis is never weight (Archivo Black has one weight; mono emphasis would muddy the readout) — it is the single-word acid color swap. Numerical content (cell numbers, stat figures, spec values) is always Archivo Black; only the cell numbers and stat figure are colored (acid / void respectively), spec values stay bone.

## Layout

### Canvas System

The system targets `100vw × 100vh` (1920×1080 fixed-stage) per slide. Default slide padding is `{spacing.pad-slide}` (72px 96px). Most slides are a vertically-centered flex column (`justify-content: center`); the content grid is top-aligned within the same padding. Only one slide is active at a time; entry is a short staggered `translateY(20px)` + opacity rise on `.reveal` children.

### Padding and Gap Scale

| Token | Value | Use |
|---|---|---|
| `{spacing.pad-slide}` | 72px 96px | Default slide padding (all archetypes) |
| `{spacing.pad-cell}` | 34px 32px 38px | Wire-grid cell internal padding |
| `{spacing.gap-spec}` | 0px | Cover spec-row gap (cells touch, divided by 1px wire rules) |
| `{spacing.max-width-body}` | 760px | Cover sub-body max width |
| `{spacing.max-width-quote}` | 1500px | Quote body max width |

### Persistent Chrome

Five elements appear on every slide (all inverting to void on the acid stat panel):
- **Top-bar** (`{components.topbar}`) — a 3px acid rule on the top edge. The upper poster trim.
- **Foot-rule** (`{components.foot-rule}`) — a 6px acid rule on the bottom edge whose width grows with slide index (≈38% → 100%). Doubles as a progress bar.
- **Brandmark** (`{components.brandmark}`) — top-left Archivo Black acid wordmark at 22px.
- **Slug** (`{components.slug}`) — top-right `// CONTEXT` mono label in muted gray.
- **Counter** (`{components.counter}`) — bottom-right `NN / NN` mono counter in muted gray.

### Surface Variations

The deck cycles through only two surfaces — the discipline is part of the identity:
- **Void content surface** — the default; carries bone display, muted body, acid accents, and wire grids. Used on 5 of 6 archetypes.
- **Full-bleed acid panel** — the stat / statement inversion only. The whole surface flips to acid with void text and inverted chrome.

### Signature Compositions

- **Cover stack** — a multi-line Archivo Black uppercase title (one acid line) over a muted mono sub-body, with a bottom `{components.spec-row}` of three wire-divided specs.
- **Section ghost** — a 220px wire section-index numeral, then a `// ` eyebrow, then the section title (one acid word), then a short acid rule.
- **Wire grid** — a 3-up `{components.wire-grid}` of `{components.grid-cell}`s, each an acid number + mono title + muted body.

## Depth and Elevation

### Flat by Mandate — No Shadows, No Gradients

The system uses **zero box-shadows and zero gradients.** Nothing floats. Depth is produced by three mechanisms only:

1. **Hard wire borders** — the 3px-outer / 1px-inner double-weight grid (`{components.wire-grid}` + `{components.grid-cell}`) and the 1px spec-row dividers. The border weights touching at intersections produce the panel-silkscreen structure.
2. **Surface inversion** — the full-bleed `{components.acid-panel}` flips the entire surface void↔acid, which reads as a hard z-jump without any shadow.
3. **Scale contrast** — a 360px stat figure or a 220px ghosted wire index against 11–15px mono metadata creates depth through sheer size hierarchy.

### The Acid Edge Frame

The persistent 3px acid top-bar and 6px acid bottom foot-rule bracket every slide top and bottom. They are flat rules, not shadows, but they create a framed-panel containment that gives the void canvas an edge. The foot-rule's growing width is the only animated depth cue.

### The Leftbar Rule

The quote cite (`{components.acid-leftbar-cite}`) is marked by a 4px acid left rule with 22px padding-left — the block reads as cantilevered off the rule with no enclosing box. This is the system's only leftbar/marker pattern.

## Shapes and Treatment

### Border Radius

- **0px on everything.** Every grid, cell, panel, CTA, leftbar, and rule is a strict rectangle. There is no exception. Rounded corners immediately collapse the front-panel brutalist register into generic web UI.

### Border Weights

- **6px solid `{colors.acid}`** — the bottom foot-rule / progress bar only.
- **4px solid `{colors.acid}`** — the leftbar cite rule only.
- **3px solid `{colors.acid}`** — the top-bar only.
- **3px solid `{colors.wire}`** — the wire-grid outer border (top + left) and the short section-title accent rule (rendered acid; 6px there).
- **1px solid `{colors.wire}`** — wire-grid inner cell borders (right + bottom) and the cover spec-row dividers.

Every border is solid; dashed and dotted borders do not exist. The weight ladder (1px / 3px / 4px / 6px) is fixed, and acid weights live only on the edge rules, the leftbar, and the CTA.

### Decorative Element Types

**Mono eyebrow (`// `)** — Acid JetBrains Mono 700 uppercase, 4px tracking, prefixed `// `. The universal section opener and the system's verbal signature.

**Acid edge frame** — A 3px acid top-bar + 6px acid bottom foot-rule on every slide; the foot-rule grows with slide index.

**Wire grid** — A 3px-outer / 1px-inner wire-bordered tabular panel of cells, each holding an acid Archivo Black number + mono title + muted body. The content archetype's structure.

**Ghosted section index** — A 140–220px Archivo Black numeral in `{colors.wire}`, sitting behind/above a section title. Reads as a faint structural watermark.

**Acid inversion panel** — A full-bleed acid surface with void Archivo Black display and inverted void chrome. The one statement move.

**Acid leftbar cite** — A 4px acid left rule + 22px padding-left holding a mono name + muted role. The quote attribution pattern.

**Acid CTA block** — A solid acid rectangle with void JetBrains Mono 700 uppercase text + trailing arrow. The closing call-to-action.

**Cover spec-row** — A 3-cell flex strip divided by 1px wire vertical rules, each a tiny mono key over an Archivo Black bone value.

**Single-word acid emphasis** — One acid-colored word inside a bone display title or mono quote. The only inline emphasis.

## Do's and Don'ts

### Do

- Use `{colors.void}` as the canvas on every slide; reserve the full-bleed `{colors.acid}` panel for the single statement/stat moment.
- Open every eyebrow and slug with `// ` in acid (eyebrow) or muted (slug) JetBrains Mono 700 uppercase. The code-comment prefix is the system signature.
- Set every display title in screaming uppercase Archivo Black with tight negative tracking and exactly one `{colors.acid}` word — no rotation.
- Render every wire grid with the 3px-outer / 1px-inner double-weight border (`{components.wire-grid}` + `{components.grid-cell}`). Cell numerals are always acid Archivo Black.
- Keep the persistent acid edge frame (3px top-bar + 6px growing foot-rule) on every slide, inverting to void on the acid panel.
- Use the `{components.acid-leftbar-cite}` (4px acid rule) for quote attributions and the solid `{components.acid-cta}` block for the closing call-to-action.
- Precede every section header with a giant ghosted `{colors.wire}` section-index numeral.
- Use JetBrains Mono 400 in `{colors.muted}` at line-height 1.7–1.75 for every body paragraph.
- Achieve all emphasis with a single-word acid color swap.

### Don't

- Don't introduce a second accent color or a sixth palette token. Acid is the only accent; void + acid is the whole identity.
- Don't round any corner — every shape is a strict rectangle. No exceptions.
- Don't add box-shadows or gradients. The system is mandated flat; depth is borders, inversion, and scale only.
- Don't rotate Archivo Black (or anything). Tilt dilutes the front-panel mass — this system's authority is weight, not movement.
- Don't substitute the faces. Archivo Black + JetBrains Mono is the pair; swapping either collapses the identity.
- Don't use Archivo Black for body or JetBrains Mono for hero display. The role split is non-negotiable.
- Don't drop the `// ` prefix on eyebrows/slugs, and don't color body text or grid borders acid.
- Don't bold or underline for emphasis — use the single-word acid swap.
- Don't crowd the stat, quote, or closing slides; they reserve large negative space around one or two huge elements.
- Don't put the stat figure on the void surface — the inversion panel is mandatory for the statement moment.

## Responsive Behavior

Voltcast is authored as a **1920×1080 presentation system**. Display sizing uses CSS `clamp()` with `vw` mid-values; borders, tracking, and chrome positions are fixed `px`. The source reference render is fixed-stage and has no mobile breakpoint of its own — it relies on the frontend-slides stage scaler to fit any viewport.

### Scaling Behavior
- Stat figure scales 160px → 360px on viewport width.
- Hero/close titles scale 64px → 168px.
- Section titles scale 48px → 96px; content titles 36px → 58px.
- Body scales 14px → 17px.
- Borders (1px / 3px / 4px / 6px), letter-spacing, and the persistent chrome offsets are fixed and do not scale.

Per the Fixed-Stage Policy above, frontend-slides renders this system at a fixed 1920×1080 stage scaled uniformly to the viewport (letterbox/pillarbox on phones) regardless of any source responsive behavior — slide content is never reflowed for mobile.

## CJK & International Content

When using this template for Chinese (or other CJK) content, swap the Latin stack for an equivalent Chinese pairing and apply the universal CJK adjustments. All recommended Chinese fonts load via CDN.

### Recommended Chinese Pairing

| Role | Latin (default) | Chinese counterpart |
|---|---|---|
| Display / hero / section / stat / cell numbers / spec values | Archivo Black 400 (ultra-heavy uppercase grotesque) | 思源黑体 Noto Sans SC 900 |
| Body / cell body / cite role | JetBrains Mono 400 (mono, muted) | 思源黑体 Noto Sans SC 400 |
| Labels / eyebrow / cell title / cite name / caption / CTA / counter | JetBrains Mono 700 (uppercase, tracked, `// ` prefix) | 思源黑体 Noto Sans SC 700 (no transform, no tracking) |

### Loading

Add to the template's `<head>`:

```html
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Noto+Sans+SC:wght@400;700;900&display=swap" rel="stylesheet">
```

### Universal CJK Adjustments

- **Line-height**: increase ~15–25% from the Latin spec. Body 1.8–1.9 (up from 1.75), display 1.0–1.15 (up from the tight 0.78–0.9). Archivo Black at 0.78 collides vertically in CJK; open to 1.0 minimum.
- **Letter-spacing**: set to 0 on every CJK run. The negative tracking on display (-2px to -10px) and the 3–4px tracking on mono labels both read as broken/gappy on square CJK glyphs.
- **Text transform**: don't apply `uppercase` to Chinese — CJK has no case. Every mono eyebrow, label, caption, cite name, and counter uses `text-transform: uppercase` in the Latin original; remove for CJK runs.
- **The `// ` prefix**: keep it (it's an ASCII glyph, language-neutral) but follow it with an ASCII space before the Chinese text.
- **Punctuation**: use full-width Chinese punctuation （，。：；！？「」）.
- **No period on display headlines**: omit trailing 。 on display-scale headlines per CJK convention.
- **盘古之白 (Pangu spacing)**: insert an ASCII space between every Chinese character and adjacent Latin character or digit. Write `±12V 模块电压` not `±12V模块电压`.
- **One font per run**: 思源黑体 covers both CJK and Latin; let it handle mixed display and body so the browser doesn't fall back to Archivo Black or JetBrains Mono mid-word.

### Aesthetic Notes for This System

The identity rests on **Archivo Black's ultra-heavy uppercase mass + the acid accent + the mono `// ` readout**. Archivo Black has no exact Chinese match; 思源黑体 Noto Sans SC 900 carries comparable density and a similarly geometric, industrial register, which suits the front-panel feel better than a serif would. The void↔acid inversion, the wire grids, the acid edge frame, and the single-word acid emphasis all survive the face swap unchanged — lean on them, since they carry most of the system's recognition. The mono readout voice softens most in CJK (no equivalent monospace personality with the tracked-uppercase stamp), so let the acid color and the `// ` prefix do the chrome-recognition work.

### Known CJK Gap

- **No CJK monospace face carries JetBrains Mono's tracked-uppercase "readout" personality.** 思源黑体 700 at 0 tracking is the closest functional match but loses the instrument-readout stamp; the acid color, the `// ` prefix, and the 1px/3px wire treatments do most of the chrome-recognition work in a CJK build.
- **Archivo Black's specific ultra-heavy grotesque has no exact Chinese counterpart.** 思源黑体 900 gives mass and industrial register but reads slightly more neutral; compensate by keeping the negative tracking off (CJK doesn't want it) and leaning on size + the acid inversion for hierarchy.

## Iteration Guide

1. Any new slide gets the persistent chrome: `{components.topbar}` (3px acid), `{components.foot-rule}` (6px acid, width = slide index / total), `{components.brandmark}`, `{components.slug}` (`// CONTEXT`), and `{components.counter}`. On an acid-panel slide, invert all five to void.
2. Any new content slide opens with a `// ` `{typography.eyebrow}` (acid) + a `{typography.content-title}` (Archivo Black uppercase, one acid word) above a `{components.wire-grid}`.
3. Any new wire-grid cell holds an acid `{typography.cell-number}` + a mono 700 `{typography.cell-label}` + a muted 400 `{typography.cell-body}`. The grid container carries 3px wire top+left; each cell carries 1px wire right+bottom.
4. Any new section header is a ghosted `{typography.section-index}` (wire) + `// ` eyebrow + `{typography.section-title}` (one acid word) + a short acid rule.
5. Any new statistic is a full-bleed `{components.acid-panel}`: void `{typography.stat-figure}` (+ `{typography.stat-unit}` if a unit) over a void `{typography.stat-caption}`, chrome inverted.
6. Any new quote is an acid Archivo Black open-mark + `{typography.quote-body}` (bone, one acid word) + an `{components.acid-leftbar-cite}` attribution.
7. Any new closing is a `// ` eyebrow + `{typography.close-title}` (one acid word) + a solid `{components.acid-cta}` block + a muted mono contact line.
8. Any new emphasis is a single-word acid color swap — never bold, never underline, never a second color.
9. If a surface feels monotone, switch it to the acid inversion panel — don't add a color or a typeface.

## Known Gaps

- **Archivo Black is a single-weight (400) face** — no lighter or bolder cuts. All display hierarchy comes from size and color; there is no way to get a "medium" display weight.
- **Both faces load from Google Fonts** via one `<link>`. With no real fallback beyond `sans-serif` / `monospace`, a Google Fonts failure collapses the identity entirely (the mass of Archivo Black and the readout of JetBrains Mono are both essential).
- **The acid green (`#C6FF00`) is extremely high-chroma.** On the full-bleed inversion panel it is intense and can vibrate against void text on low-quality displays; it is intended as a punctuating moment, not a surface to dwell on — keep acid panels to one per deck section.
- **The wire grid uses overlapping border weights** (3px outer + 1px inner). Rendering is generally clean but can produce sub-pixel seams at certain zoom levels.
- **The foot-rule width is content-authored** (a percentage per slide), not computed — a generator must set each slide's foot-rule width manually to keep the progress cue monotonic.
- **Body text in `{colors.muted}` on `{colors.void}` is a deliberately recessive contrast.** It is readable at presentation scale but should not be used for long-form reading; keep body to short paragraphs.
- **The single-word acid emphasis assumes one emphasis target per title.** Titles needing two emphasized words have no second mechanism — the system has no bold or underline fallback.
