---
version: alpha
name: Stagehand Dev
description: "A developer-tools landing-page system in the lineage of modern SDK and open-source homepages (Vercel, Browserbase Stagehand, Railway). Its thesis is structural, not typographic: a 1px DASHED-BORDER grid is the signature — a dashed frame insets every slide, a faint 80px dashed graph-paper grid underlays cream surfaces, and cards/dividers/buttons are all ruled in 1px dashes rather than solid lines or shadows. The single brand accent is a golden yellow (#F5A623); a secondary spectrum of red/blue/green/purple appears ONLY inside isometric 3D cube graphics drawn with diagonal line-hatching on one face. Type is the authentic dev pairing: Inter (600 display, 400 body) for everything human-readable, JetBrains Mono for every label, breadcrumb, code block, stat, and chrome detail — the mono carries the 'terminal' voice (`// EYEBROWS`, `~/breadcrumbs`, `$ commands`). Surfaces alternate between warm cream (#F7F4EF) content slides and charcoal (#1F1F1F) sections carrying an feTurbulence noise texture and dashed-light borders. The register is flat, technical, precise, and confidently under-decorated — square 8px radii, zero drop shadows, no gradients."

colors:
  bg: "#F7F4EF"
  dark: "#1F1F1F"
  card: "#FFFFFF"
  muted: "#E8E4DD"
  ink: "#1A1A1A"
  ink-soft: "#3A372F"
  ink-mute: "#8A857B"
  primary: "#F5A623"
  primary-dark: "#D4900F"
  code-bg: "#F0ECE3"
  accent-red: "#E74C3C"
  accent-blue: "#3498DB"
  accent-green: "#27AE60"
  accent-purple: "#9B59B6"

typography:
  eyebrow:
    fontFamily: "'JetBrains Mono', monospace"
    fontWeight: 500
    fontSize: "15px"
    letterSpacing: "3px"
    textTransform: "uppercase"
    color: "{colors.primary-dark}"
  hero-title:
    fontFamily: "'Inter', sans-serif"
    fontWeight: 600
    fontSize: "clamp(56px, 6.4vw, 92px)"
    lineHeight: 1.04
    letterSpacing: "-0.02em"
    color: "{colors.ink}"
  h1:
    fontFamily: "'Inter', sans-serif"
    fontWeight: 600
    fontSize: "clamp(44px, 5vw, 78px)"
    lineHeight: 1.08
    letterSpacing: "-0.015em"
    color: "{colors.ink}"
  h2:
    fontFamily: "'Inter', sans-serif"
    fontWeight: 600
    fontSize: "clamp(28px, 2.8vw, 40px)"
    lineHeight: 1.2
    letterSpacing: "-0.01em"
    color: "{colors.ink}"
  card-title:
    fontFamily: "'Inter', sans-serif"
    fontWeight: 600
    fontSize: "26px"
    lineHeight: 1.25
    color: "{colors.ink}"
  body:
    fontFamily: "'Inter', sans-serif"
    fontWeight: 400
    fontSize: "21px"
    lineHeight: 1.6
    color: "{colors.ink-soft}"
  small:
    fontFamily: "'Inter', sans-serif"
    fontWeight: 400
    fontSize: "16px"
    lineHeight: 1.5
    color: "{colors.ink-mute}"
  quote:
    fontFamily: "'Inter', sans-serif"
    fontWeight: 600
    fontSize: "clamp(36px, 3.6vw, 52px)"
    lineHeight: 1.28
    letterSpacing: "-0.01em"
    color: "{colors.ink}"
  stat-number:
    fontFamily: "'Inter', sans-serif"
    fontWeight: 700
    fontSize: "clamp(80px, 8.5vw, 120px)"
    lineHeight: 0.9
    letterSpacing: "-0.03em"
    color: "{colors.primary}"
  stat-label:
    fontFamily: "'JetBrains Mono', monospace"
    fontWeight: 400
    fontSize: "16px"
    letterSpacing: "2px"
    textTransform: "uppercase"
    color: "rgba(244,241,236,0.6)"
  section-numeral:
    fontFamily: "'JetBrains Mono', monospace"
    fontWeight: 700
    fontSize: "clamp(160px, 16vw, 240px)"
    lineHeight: 0.8
    color: "transparent"
    webkitTextStroke: "2px {colors.ink}"
  wordmark:
    fontFamily: "'JetBrains Mono', monospace"
    fontWeight: 700
    fontSize: "18px"
    letterSpacing: "0.5px"
    color: "{colors.ink}"
  crumb:
    fontFamily: "'JetBrains Mono', monospace"
    fontWeight: 400
    fontSize: "13px"
    letterSpacing: "1px"
    color: "{colors.ink-mute}"
  meta-mono:
    fontFamily: "'JetBrains Mono', monospace"
    fontWeight: 400
    fontSize: "13px"
    letterSpacing: "2px"
    color: "{colors.ink-mute}"
  card-tag:
    fontFamily: "'JetBrains Mono', monospace"
    fontWeight: 400
    fontSize: "13px"
    letterSpacing: "2px"
    textTransform: "uppercase"
    color: "{colors.ink-mute}"
  code:
    fontFamily: "'JetBrains Mono', monospace"
    fontWeight: 400
    fontSize: "18px"
    lineHeight: 1.7
    color: "{colors.ink}"
  btn-label:
    fontFamily: "'Inter', sans-serif"
    fontWeight: 600
    fontSize: "19px"
    color: "{colors.ink}"
  cmd-mono:
    fontFamily: "'JetBrains Mono', monospace"
    fontWeight: 500
    fontSize: "18px"
    color: "{colors.ink}"

spacing:
  frame-inset: "56px"
  pad-slide: "120px"
  topbar-height: "72px"
  gap-card-grid: "28px"
  pad-card: "34px 32px"
  pad-code: "22px 26px"
  pad-button: "16px 28px"
  radius: "8px"
  radius-sm: "4px"
  grid-cell: "80px"

canvas:
  width: 100vw
  height: 100vh
  background: "{colors.bg}"

components:
  dashed-frame:
    border: "1px dashed {colors.ink}"
    inset: "56px"
    borderRadius: "8px"
    description: "The system's signature: a 1px dashed rectangle inset 56px from every slide edge, framing all content. On dark surfaces it becomes 1px dashed rgba(255,255,255,0.28). Present on every archetype — it is the single most recognizable element."
  grid-underlay:
    background: "repeating-linear-gradient 80px cells, rgba(26,26,26,0.045)"
    description: "Faint graph-paper grid of 80px cells drawn in two repeating-linear-gradients (90deg + 0deg) at ~4.5% ink opacity. Underlays every cream surface beneath the dashed frame. Provides the 'engineering drawing' substrate; never appears on dark surfaces (replaced by noise there)."
  topbar:
    height: "72px"
    borderBottom: "1px dashed {colors.ink}"
    description: "Persistent header strip inside the frame: brand wordmark (+ optional cube logo) at left, a mono breadcrumb or version string at right, separated from the slide body by a 1px dashed bottom rule. The deck's primary chrome."
  feature-card:
    background: "{colors.card}"
    border: "1px dashed {colors.ink}"
    borderRadius: "8px"
    padding: "34px 32px"
    description: "White card with a 1px dashed border and 8px radius, NO shadow. Holds an isometric cube icon (top), an Inter 600 card-title, an Inter 400 small body, and a bottom-anchored JetBrains Mono card-tag (// LABEL). The system's primary content unit."
  isometric-cube:
    description: "Hand-built SVG cube in 2:1 isometric projection: a top rhombus face in an accent color, a near-black (#1A1A1A) left face, and a right face that is EITHER the accent at 45% opacity OR filled with a 45deg diagonal line-hatch pattern (1.4px ink strokes, 9px pitch). All edges stroked 4-7px solid ink. The system's only illustrative motif — cubes cluster in stacks of 1-3 at varying scales."
  code-block:
    background: "{colors.code-bg}"
    border: "1px dashed {colors.ink}"
    borderRadius: "8px"
    padding: "22px 26px"
    description: "Light warm-gray (#F0ECE3) panel, 1px dashed border, monospace contents with token-colored syntax: keywords purple, strings green, function calls blue, comments mute-gray. On dark surfaces the ground becomes rgba(255,255,255,0.04) with a dashed-light border."
  btn-primary:
    background: "{colors.primary}"
    border: "1px solid {colors.ink}"
    borderRadius: "4px"
    padding: "16px 28px"
    description: "Golden-yellow filled button with a 1px SOLID ink border (the one place solid borders are used over dashed) and a mono → arrow. Carries Inter 600 ink-colored label. The single primary CTA style."
  btn-dashed:
    border: "1px dashed {colors.ink}"
    borderRadius: "4px"
    padding: "16px 28px"
    description: "Transparent secondary button with a 1px dashed border and JetBrains Mono label — almost always a shell command ($ npm i …). The dashed outline ties it to the frame/card system."
  noise-overlay:
    description: "feTurbulence fractalNoise (baseFrequency 0.65, 3 octaves) tiled at 240px over dark surfaces at ~50% opacity with mix-blend-mode screen, giving charcoal panels a fine film-grain texture. Applied only on {colors.dark} sections."
  accent-bar:
    background: "{colors.primary}"
    border: "1px solid {colors.ink}"
    description: "A short golden-yellow vertical bar (≈8px wide) with a 1px solid ink outline, used to mark a quote attribution or flag an emphasis block. A compact echo of the primary button's fill+outline treatment."
  stat-divider:
    borderRight: "1px dashed rgba(255,255,255,0.28)"
    description: "Vertical 1px dashed-light rule separating big stat figures on dark statement slides. Each stat cell is padded and divided — never boxed."
---

## Frontend Slides Fixed-Stage Policy

When this design system is used by the `frontend-slides` skill, generate the final deck as a **fixed 1920×1080 stage** that scales uniformly to the browser viewport. The deck should preserve a 16:9 slide canvas on every screen, including phones; it may letterbox or pillarbox, but it should not reflow slide content for mobile.

This policy has higher priority than any source-template responsive behavior described later in this file. If a later section says the original template is viewport-fluid, treat that as source history only, not as the target generation model for `frontend-slides`.

This policy applies even if values below use `100vw`, `100vh`, `vw`, `vh`, or `clamp()`. Treat those as design proportions to translate into 1920×1080 stage coordinates, not as live responsive rules in the generated deck.

Render each slide at 1920×1080, scale the whole stage with one transform, and verify rendered screenshots for both text overflow and panel overlap.

## Overview

Stagehand Dev is a **developer-tools landing-page system** — the visual language of a modern SDK or open-source-framework homepage, brought to slides. Its closest cousins are the homepages of Vercel, Railway, and Browserbase's Stagehand: warm-neutral grounds, an engineering-drawing grid, one confident accent, and small monospace details that signal "this was made by people who ship code." The premise is that a technical deck should feel like documentation you trust — precise, structured, under-decorated — not like a marketing deck dressed in gradients.

The thesis is **structural, not typographic**. The signature move is the **1px dashed border**, used as a complete system: a dashed rectangle insets 56px from every slide edge and frames all content; a faint 80px graph-paper grid underlays every cream surface beneath it; the persistent top bar is divided from the body by a dashed rule; and every card, divider, secondary button, and code block is ruled in 1px dashes rather than solid lines or drop shadows. Where other systems reach for elevation or color blocking, this one reaches for a dashed line. The discipline is what reads as "engineered."

The **type system** is the authentic developer pairing: **Inter** and **JetBrains Mono**, each in a strict role. Inter handles everything a human reads as prose — hero titles and section headers at weight 600 with tight negative tracking (−0.015 to −0.03em), body and card copy at weight 400. JetBrains Mono handles everything that signals "machine": the `// UPPERCASE` eyebrows, the `~/breadcrumb` and `NN / NN` chrome, the `$ shell` command buttons, the syntax-highlighted code blocks, the stat labels, and the giant outlined section numerals. The mono is the system's "terminal voice" — it is never used for prose, and Inter is never used for a label. This split is the rule that keeps the system feeling like a dev tool rather than a generic SaaS deck.

The **color philosophy** is one accent, strictly held. Golden yellow (`{colors.primary}` — `#F5A623`) is the only brand color: it fills the single primary CTA, colors the eyebrow labels (as the darker `{colors.primary-dark}` on light grounds), and drives every big stat figure. It is never used as body text, never as a card fill, never as a second structural color. A **secondary spectrum** — red, blue, green, purple — exists but is quarantined: it appears *only* inside the isometric cube graphics (one accent per cube face), never as UI color. Surfaces alternate between warm cream (`{colors.bg}` — `#F7F4EF`) content slides and charcoal (`{colors.dark}` — `#1F1F1F`) statement/closing sections, the latter carrying a fine feTurbulence noise texture and dashed-light borders.

**Depth is flat by commitment.** There are no drop shadows and no gradients anywhere in the system. Depth is implied three ways only: the dashed/solid border ladder, the surface inversion (cream ↔ noisy charcoal), and the isometric cubes' three-face shading. Corners are square-ish — an 8px radius on frames/cards/code, 4px on buttons — never pill-rounded. **Density is medium**: content slides carry a 3-column card grid plus a code block and still breathe; statement slides drop to three big stats or one cream-ground quote with generous negative space. The system reads as confident precisely because it refuses to over-fill.

**Key Characteristics:**
- A 1px **dashed border** is the signature, applied as a full system: a 56px-inset slide frame, a dashed top-bar rule, dashed cards, dashed dividers, dashed secondary buttons, and a dashed-bordered code block.
- A faint **80px graph-paper grid** (≈4.5% ink) underlays every cream surface — the "engineering drawing" substrate.
- **Isometric 3D cubes** drawn as SVG with a hatched or half-opacity right face are the only illustrative motif; they cluster in stacks of 1-3 at varying scale.
- **Golden yellow** (`{colors.primary}`) is the single brand accent; a red/blue/green/purple spectrum is allowed *only* inside cubes.
- **Inter + JetBrains Mono** in strict roles: Inter for all prose/display, JetBrains Mono for every label, breadcrumb, command, code block, and numeral.
- **Cream ↔ noisy charcoal** surface alternation; dark surfaces carry an feTurbulence film-grain and switch borders to dashed-light.
- **Mono chrome** on every slide: brand wordmark, a `~/breadcrumb` page tag, a `NN / NN` counter in a dashed-cornered tab.
- **Zero drop shadows, zero gradients** — depth comes from borders, surface inversion, and isometric shading only.
- **Square radii** — 8px on frames/cards/code, 4px on buttons; nothing is pill-rounded.
- The one place a **solid** border replaces dashed is the **primary yellow button** (1px solid ink) and the small accent bar — a deliberate signal that "this is the action."

## Colors

### Palette

**Core (structural) palette — the system commits to these five:**

- **Bg** (`{colors.bg}` — `#F7F4EF`): Warm cream. The default content-slide ground. Reads as recycled-paper / engineering vellum. Forbidden as a text color on light surfaces.
- **Dark** (`{colors.dark}` — `#1F1F1F`): Charcoal. The statement/closing-slide ground, always carrying the noise overlay and dashed-light borders. Not a text color.
- **Card** (`{colors.card}` — `#FFFFFF`): Pure white, used only as the fill of feature cards so they lift a half-step off the cream ground without a shadow. Never a full-slide ground (that's `bg`).
- **Ink** (`{colors.ink}` — `#1A1A1A`): Near-black. Every border, every dash, every display headline, every wordmark. The system's line and text color on light surfaces.
- **Primary** (`{colors.primary}` — `#F5A623`): Golden yellow. The single brand accent — primary CTA fill, big stat figures, eyebrows (as `primary-dark` on light grounds, `primary` on dark). Never body text, never a card fill, never a structural second color.

**Supporting tints (derived from ink, not new hues):** `{colors.ink-soft}` (`#3A372F`) for body prose, `{colors.ink-mute}` (`#8A857B`) for mono chrome and captions, `{colors.muted}` (`#E8E4DD`) and `{colors.code-bg}` (`#F0ECE3`) for subtle panel fills, `{colors.primary-dark}` (`#D4900F`) for eyebrows and the hover/darker yellow.

**Icon spectrum — quarantined to cubes only:** `{colors.accent-red}` (`#E74C3C`), `{colors.accent-blue}` (`#3498DB`), `{colors.accent-green}` (`#27AE60`), `{colors.accent-purple}` (`#9B59B6`). These give isometric cubes and code syntax tokens their variety. They must **never** appear as UI accents, button fills, borders, or text emphasis — the moment one colors a heading, the single-accent discipline breaks.

### Defaults

- **Default surface background**: `{colors.bg}` (cream) with the grid underlay. Switch to `{colors.dark}` (+ noise) for stat/statement and closing slides.
- **Default headline / display color**: `{colors.ink}` on cream, `#F4F1EC` (near-white) on charcoal. Headlines are never yellow — only stat figures are.
- **Default body text color**: `{colors.ink-soft}` on cream, `rgba(244,241,236,0.72)` on charcoal.
- **Default eyebrow color**: `{colors.primary-dark}` on cream, `{colors.primary}` on charcoal. Always JetBrains Mono, uppercase, 3px tracking, prefixed `//`.
- **Default border / dash color**: `{colors.ink}` on cream, `rgba(255,255,255,0.28)` on charcoal.
- **Default big-number color**: `{colors.primary}` (golden yellow). Every stat figure is yellow; the unit suffix (`ms`, `%`) rides along smaller in the same yellow.
- **Default card fill**: `{colors.card}` (white). The code block is the one panel that fills `{colors.code-bg}` instead.

Commit hard to **one accent**. Do not add a second UI color for "positive/negative/info." Categorical differentiation comes from the mono labels, the cube colors, and surface inversion — never from a new brand hue.

## Typography

### Font Family Stack

The system runs two families in strict, non-overlapping roles.

**Inter** (Google Fonts, weights 400/500/600/700) is the **human voice** — everything a reader reads as language. Hero titles and section headers are Inter 600 with tight negative letter-spacing (−0.015 to −0.03em) so large type sets densely and "engineered." Body and card copy are Inter 400 at 1.5–1.6 line-height. Inter is never used for a label, a breadcrumb, a command, or a numeral.

**JetBrains Mono** (Google Fonts, weights 400/500/700) is the **machine voice** — every signal that the artifact is technical. It sets the `// UPPERCASE` eyebrows (500, 3px tracking), the brand wordmark (700), the `~/breadcrumb` page tags and `NN / NN` counters (400, 1–2px tracking), the `$ shell` command buttons (500), the code blocks (400, with syntax coloring), the stat labels (400, 2px tracking, uppercase), and the giant outlined section numerals (700, transparent fill + ink stroke). JetBrains Mono is never used for prose.

The role split is the system's identity guardrail: Inter prose ↔ Mono chrome. Cross them and the deck stops reading as a dev tool.

### Typography Scale

| Token | Size (clamp / px) | Family | Weight | Use |
|---|---|---|---|---|
| `{typography.section-numeral}` | 160–240px | JetBrains Mono | 700 | Giant outlined (stroke-only) numeral on section-header slides |
| `{typography.stat-number}` | 80–120px | Inter | 700 | Big stat figure, always golden yellow, on dark statement slides |
| `{typography.hero-title}` | 56–92px | Inter | 600 | Cover/hero headline (tightest tracking, −0.02em) |
| `{typography.h1}` | 44–78px | Inter | 600 | Section-header and closing headline |
| `{typography.quote}` | 36–52px | Inter | 600 | Pull-quote body on a cream quote slide |
| `{typography.h2}` | 28–40px | Inter | 600 | Content-slide title above a card grid |
| `{typography.card-title}` | 26px | Inter | 600 | Feature-card title (often a code identifier like `act()`) |
| `{typography.body}` | 21px | Inter | 400 | Standard body paragraph (ink-soft) |
| `{typography.btn-label}` | 19px | Inter | 600 | Primary-button label |
| `{typography.cmd-mono}` | 18px | JetBrains Mono | 500 | Dashed-button shell command ($ …) |
| `{typography.code}` | 18px | JetBrains Mono | 400 | Code-block contents (syntax-colored) |
| `{typography.wordmark}` | 18px | JetBrains Mono | 700 | Brand wordmark in the top bar |
| `{typography.small}` | 16px | Inter | 400 | Card body and caption copy (ink-mute) |
| `{typography.stat-label}` | 16px | JetBrains Mono | 400 | Uppercase label under a stat figure |
| `{typography.eyebrow}` | 15px | JetBrains Mono | 500 | `// UPPERCASE` section eyebrow, 3px tracking |
| `{typography.crumb}` | 13px | JetBrains Mono | 400 | Top-bar breadcrumb / version string |
| `{typography.meta-mono}` | 13px | JetBrains Mono | 400 | `~/path` page tag and `NN / NN` counter |
| `{typography.card-tag}` | 13px | JetBrains Mono | 400 | Bottom-anchored `// LABEL` inside a card, 2px tracking |

### Defaults

- **Default cover headline**: `{typography.hero-title}` (Inter 600, 56–92px, −0.02em), preceded by a `{typography.eyebrow}` mono label.
- **Default section opener**: a `{typography.section-numeral}` outlined numeral beside an `{typography.h1}` title, divided by a dashed vertical rule.
- **Default content-slide title**: `{typography.h2}` over a 3-card grid.
- **Default body**: `{typography.body}` (Inter 400, 21px, line-height 1.6) in `{colors.ink-soft}`; card body drops to `{typography.small}` (16px) in `{colors.ink-mute}`.
- **Default eyebrow**: `{typography.eyebrow}` — JetBrains Mono 500, uppercase, 3px tracking, always prefixed with `//`.
- **Default big number**: `{typography.stat-number}` (Inter 700) in `{colors.primary}`.
- **Default mono chrome**: `{typography.crumb}` / `{typography.meta-mono}` in `{colors.ink-mute}`.

When unsure which display token to reach for, default to `{typography.h2}` for a content-slide opener and reserve `{typography.hero-title}` for the cover and `{typography.section-numeral}` for true section dividers.

### Signature Treatments

These are **non-optional whenever the element type appears**:

- **Every eyebrow is JetBrains Mono, uppercase, 3px-tracked, and prefixed `//`** (e.g. `// THE BROWSER AUTOMATION SDK`). The slash prefix is the system's "comment" signal — an eyebrow without it reads as a generic kicker.
- **Every big stat figure is Inter 700 in `{colors.primary}` (golden yellow), with any unit suffix riding smaller in the same yellow.** Stats are the only yellow text in the system; a dark stat figure breaks the data-signal hierarchy.
- **Every section-divider numeral is the outlined treatment**: JetBrains Mono 700, `color: transparent`, `-webkit-text-stroke: 2px {colors.ink}`. A solid-filled numeral collapses the engineering-drawing feel.
- **Every shell-command button uses JetBrains Mono with a literal `$ ` prefix** inside a dashed button. The command-as-button is the system's secondary CTA.
- **Hero/section headlines carry tight negative tracking** (−0.015 to −0.03em). Inter at default tracking reads as generic SaaS; the negative tracking is what makes it read as "set with care."
- **Body and card prose never go yellow and never go mono.** Prose is Inter in ink tints, full stop.

## Layout

### Canvas System

Each slide is a 1920×1080 stage. Content lives inside a **56px-inset dashed frame** (`{components.dashed-frame}`); nothing but the letterbox sits outside it. The first interior band is the **72px top bar** (`{components.topbar}`) holding brand at left and a mono breadcrumb at right, closed by a dashed bottom rule. The slide body begins below it. Persistent chrome at the bottom: a `~/path` page tag at lower-left and an `NN / NN` counter in a dashed-cornered tab at lower-right.

### Padding and Gap Scale

| Token | Value | Use |
|---|---|---|
| `{spacing.frame-inset}` | 56px | Inset of the dashed frame and top bar from the slide edge |
| `{spacing.topbar-height}` | 72px | Height of the persistent top bar |
| `{spacing.pad-slide}` | 120px | Left content margin for hero/section/closing bodies |
| `{spacing.gap-card-grid}` | 28px | Gap between feature cards in the 3-column grid |
| `{spacing.pad-card}` | 34px 32px | Internal padding of a feature card |
| `{spacing.pad-code}` | 22px 26px | Internal padding of a code block |
| `{spacing.pad-button}` | 16px 28px | Button padding (both primary and dashed) |
| `{spacing.grid-cell}` | 80px | Cell size of the graph-paper grid underlay |

### Persistent Chrome

Three elements recur on every slide, all inside the frame:
- **Top bar** — brand wordmark (cover/closing add the cube logo) at left; a mono breadcrumb, version string, or section name at right; dashed bottom rule.
- **Page tag** — a `~/path`-style JetBrains Mono string at lower-left (`~/architecture`, `~/benchmarks`), reinforcing the "filesystem" metaphor.
- **Counter** — `NN / NN` in a small tab whose top and left edges are dashed, at lower-right.

### Surface Variations

The deck cycles through three surfaces:
- **Cream content surface** (default) — `{colors.bg}` + grid underlay + dashed ink chrome. Hero, section, content, quote.
- **Charcoal statement surface** — `{colors.dark}` + noise overlay + dashed-light chrome + near-white text. Stat slides and the closing slide. Yellow stats pop hardest here.
- **White card fill** — only inside feature cards, to lift them off the cream without a shadow.

### Signature Compositions

- **Hero**: left-aligned eyebrow → two-line Inter 600 headline → body → dual CTA (yellow primary + dashed command), with an isometric cube cluster floated to the right third.
- **Section header**: a giant outlined numeral at far left, a dashed vertical rule, then eyebrow + multi-line `{typography.h1}` + lead, right of the rule.
- **Content**: `{typography.h2}` title → 3-column dashed card grid (each card = cube icon + title + body + `// TAG`) → a full-width dashed code block beneath.
- **Stat**: eyebrow + statement headline → a 3-up row of yellow `{typography.stat-number}` figures divided by dashed-light vertical rules.
- **Quote**: an oversized yellow outlined `"` glyph → `{typography.quote}` → an accent-bar attribution, with a single hatched cube to the right.

## Depth and Elevation

### Flat by Commitment

The system has **zero box-shadows and zero gradients**. Cards do not float; panels do not glow. This flatness is a deliberate identity choice — the dev-tool register depends on it.

### The Three Depth Mechanisms

Depth is implied only through:

1. **The border ladder.** A 1px dashed line is the default edge for frames, cards, dividers, code blocks, and secondary buttons. A 1px *solid* ink line is reserved for the primary yellow button and the small accent bar — the solidity is itself a depth/importance signal ("this is the action"). Cube edges step up to 4–7px solid ink strokes so the illustration reads as built, not drawn.

2. **Surface inversion.** Switching the whole ground from cream (+grid) to charcoal (+noise) is the system's biggest "elevation" move — it changes the plane rather than lifting an element off it. Reserve it for statement and closing moments.

3. **Isometric shading.** The cubes carry the only literal 3D in the system: a lit top face (accent color), a shadowed left face (near-black `#1A1A1A`), and a right face that is either the accent at 45% opacity or filled with diagonal hatching. The three-value shading is what makes a flat SVG read as a solid object.

### White-on-Cream Card Lift

Feature cards fill pure white on the cream ground. The half-step value difference (cream → white) plus the dashed border is enough separation — adding a shadow here would immediately break the system.

## Shapes and Treatment

### Border Radius

- **8px** (`{spacing.radius}`) on the dashed frame, feature cards, and code block.
- **4px** (`{spacing.radius-sm}`) on buttons.
- **0px** on dividers, accent bars, and cube faces.

Nothing is pill-rounded. The slightly-rounded-but-mostly-square radius is part of the technical register; fully rounded "bubble" cards collapse it into consumer-app aesthetic.

### Border Weights

- **1px dashed `{colors.ink}`** — the default: frame, top-bar rule, cards, code block, dividers, secondary buttons. (`rgba(255,255,255,0.28)` dashed on dark surfaces.)
- **1px solid `{colors.ink}`** — primary yellow button and accent bar only.
- **4–7px solid `{colors.ink}`** — isometric cube edges (heavier on larger cubes).
- **1.4px solid `{colors.ink}`** — the diagonal hatch strokes inside a cube's right face (9px pitch, 45°).

The dashed-vs-solid distinction is load-bearing: **dashed = structure/decoration, solid = action/object.** Keep them separated.

### Decorative Element Types

**Dashed frame** — 1px dashed rectangle inset 56px, 8px radius. The signature; present on every slide.

**Graph-paper grid** — 80px-cell repeating-linear-gradient underlay at ~4.5% ink, on cream surfaces only.

**Isometric cube** — SVG cube in 2:1 iso projection: accent top face, near-black left face, hatched-or-45%-accent right face, 4–7px ink edges. Clusters of 1–3 at varying scale. The only illustration.

**Diagonal hatch** — 45° line pattern (1.4px ink strokes, 9px pitch) filling a cube's right face; the "technical drawing" fill that distinguishes these cubes from generic flat-3D icons.

**Noise overlay** — feTurbulence fractalNoise (baseFrequency 0.65, 3 octaves) tiled 240px at ~50% opacity, screen-blended, on charcoal surfaces only.

**Outlined numeral** — stroke-only JetBrains Mono 700 numeral (transparent fill, 2px ink stroke) for section dividers.

**Accent bar** — short yellow vertical bar with a 1px solid ink outline, marking quote attributions / emphasis.

**Mono chrome set** — wordmark, `~/path` page tag, `NN / NN` dashed-corner counter — the recurring "terminal" furniture.

## Do's and Don'ts

### Do

- Frame every slide with the 56px-inset 1px dashed rectangle (`{components.dashed-frame}`) and underlay cream surfaces with the 80px graph-paper grid. The dashed-grid pairing is the system's identity.
- Keep golden yellow (`{colors.primary}`) as the only brand accent — primary CTA fill, big stats, eyebrows. Achieve all other differentiation through mono labels and surface inversion.
- Set every eyebrow in JetBrains Mono, uppercase, 3px-tracked, prefixed `//`. Set every breadcrumb/counter/command/code block in JetBrains Mono too — keep prose in Inter.
- Use isometric cubes (with a hatched or 45%-opacity right face) as the illustration motif, and let the red/blue/green/purple spectrum live *only* inside them.
- Alternate cream content surfaces with noisy-charcoal statement surfaces; switch borders to dashed-light on dark grounds.
- Reserve the 1px *solid* border for the primary yellow button and accent bar; everything else is dashed.
- Make big stat figures Inter 700 in yellow, with the unit suffix smaller in the same yellow.
- Render the section-divider numeral as outline-only (transparent fill + 2px ink stroke).
- Keep radii square-ish: 8px on frames/cards/code, 4px on buttons.

### Don't

- Don't add a second UI accent. Red/blue/green/purple are cube-and-syntax colors only — never a heading, button, border, or emphasis color.
- Don't add drop shadows or gradients. Depth is borders + surface inversion + isometric shading, nothing else. A shadowed card breaks the system instantly.
- Don't make borders solid by default. Dashed = structure; solid is reserved for the action (yellow button) and the object (cube edges).
- Don't set prose in JetBrains Mono or labels in Inter. The Inter-prose ↔ Mono-chrome split is non-negotiable.
- Don't color a headline yellow. Only stat figures are yellow; headlines are ink (or near-white on dark).
- Don't pill-round corners or use large radii. The square-ish radius is part of the technical register.
- Don't put the graph-paper grid on dark surfaces or the noise on cream ones — each surface has its own texture.
- Don't drop the `//` on eyebrows or the `$`/`~/` on commands and page tags. The terminal punctuation is the system's voice.
- Don't over-decorate the cubes (no more than three per composition; no gradients on faces) — the hatch + three-value shading is the whole effect.

## Responsive Behavior

Stagehand Dev is authored as a **1920×1080 presentation system**. Display type uses `clamp()` with `vw` mid-values; borders, dashes, chrome, and the grid/hatch pitches are fixed `px`. Per the Fixed-Stage Policy above, `frontend-slides` renders one fixed 1920×1080 stage scaled by a single transform — the responsive notes here are source history, not a generation target.

### Scaling Behavior (source history)
- Hero title scales 56px → 92px; h1 44px → 78px; quote 36px → 52px.
- Stat figures scale 80px → 120px; section numerals 160px → 240px.
- Body (21px), card body (16px), and all mono chrome (13–18px) are fixed.
- Frame inset (56px), dash weights (1px), card/grid gaps, the 80px grid pitch, and cube stroke weights are fixed and do not scale.

### Original Mobile Intent
The source dev-landing language collapsed the 3-column card grid to 1 column, stacked the stat row vertically, and dropped the right-hand cube cluster below the hero on narrow viewports. In `frontend-slides` these do not apply — the deck letterboxes at 16:9 instead of reflowing.

## CJK & International Content

The Latin pairing (Inter / JetBrains Mono) has clean, well-matched CJK counterparts, so this system localizes well. All recommended fonts load via Google Fonts CDN.

### Recommended CJK Pairing

| Role | Latin (default) | CJK counterpart |
|---|---|---|
| Display / headline / card title / stat figure (Inter 600–700) | Inter | 思源黑体 Noto Sans SC 700/900 |
| Body / caption (Inter 400) | Inter | 思源黑体 Noto Sans SC 400 |
| Eyebrow / breadcrumb / command / code / counter / numeral (JetBrains Mono) | JetBrains Mono | Latin JetBrains Mono for ASCII; 更紗黑体 Sarasa Mono SC for any CJK that must sit in a monospace run |

The system is sans-led, so Noto Sans SC carries both display and body (hierarchy comes from weight, size, and the yellow accent — exactly as in the Latin original). Sarasa Mono SC is a CJK-aware monospace that preserves the terminal voice when a label or code comment contains Chinese; pure-ASCII chrome (`// LABEL`, `$ npm i`, `~/path`, `NN / NN`, numerals) should stay in JetBrains Mono.

### Loading

```html
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&family=JetBrains+Mono:wght@400;500;700&family=Noto+Sans+SC:wght@400;500;700;900&display=swap" rel="stylesheet">
```

### Universal CJK Adjustments

- **Line-height**: raise by ~15%. Body 1.7–1.8 (from 1.6), display 1.15–1.25 (from the tight 1.04–1.2). The negative letter-spacing on Latin display must go to 0 for CJK.
- **Letter-spacing**: set to 0 on every CJK run. The −0.02em display tracking and the 2–3px mono tracking both read wrong on square CJK glyphs. Keep the tracking only on ASCII chrome that stays in JetBrains Mono.
- **Text transform**: don't apply `uppercase` to CJK — it has no case. The eyebrow's `//` prefix stays, but drop the uppercase transform; keep the ASCII portion (`//`, latin words) uppercase if mixed.
- **Punctuation**: use full-width Chinese punctuation （，。：；！？「」） in prose; keep half-width ASCII in code blocks and commands.
- **盘古之白**: insert a space between CJK characters and adjacent Latin/digits (write `Stagehand 浏览器自动化`, not `Stagehand浏览器自动化`).
- **Terminal furniture stays Latin**: the `// `, `$ `, `~/`, and `NN / NN` chrome are part of the dev-tool identity — keep them ASCII even in a CJK deck.

### Known CJK Gap

- **The `//` `$` `~/` terminal punctuation has no CJK equivalent** and is the system's strongest voice signal; in a CJK build it must remain ASCII, which produces deliberate Latin/CJK mixing in chrome. This is on-brand (code is written in ASCII) but worth a conscious choice.
- **Inter's tight negative tracking is a Latin-only move**; Noto Sans SC at 0 tracking loses a little of the "set with care" density. Compensate by leaning on weight contrast (900 display vs 400 body) and the yellow accent.

## Iteration Guide

1. Any new slide starts with the 56px dashed frame + top bar; cream surfaces add the 80px grid underlay, dark surfaces add the noise overlay and switch chrome to dashed-light.
2. Any new section divider uses an outlined `{typography.section-numeral}` at far left + a dashed vertical rule + eyebrow + `{typography.h1}`.
3. Any new content slide is a `{typography.h2}` title over a 3-column `{components.feature-card}` grid; add a full-width `{components.code-block}` beneath if a code example helps.
4. Any new feature card = isometric cube icon (top) + `{typography.card-title}` + `{typography.small}` body + bottom-anchored `{typography.card-tag}` (`// LABEL`).
5. Any new statistic is `{typography.stat-number}` in `{colors.primary}` with a `{typography.stat-label}` beneath; group 2–4 across a dark surface divided by `{components.stat-divider}` dashed-light rules.
6. Any new CTA pairs the `{components.btn-primary}` (yellow, solid border, → arrow) with a `{components.btn-dashed}` shell command (`$ …`).
7. Any new eyebrow is JetBrains Mono uppercase, 3px-tracked, `//`-prefixed; any new breadcrumb/page-tag is JetBrains Mono with `~/` or section-name styling.
8. Any new illustration is an isometric cube (or 2–3 clustered): assign one icon-spectrum color to the top face, near-black to the left, hatch-or-45% to the right.
9. If a slide feels flat or monotone, switch the *surface* (cream → noisy charcoal) rather than adding a color or a shadow.
10. Keep yellow scarce: if more than the CTA, the eyebrow, and the stats are yellow on a slide, pull some back to ink.

## Known Gaps

- **Inter and JetBrains Mono are widely-used faces, not exotic display fonts.** This system's distinctiveness is deliberately structural — the dashed-grid frame, isometric hatched cubes, single-yellow discipline, and terminal punctuation carry the identity, not the type. Swapping the fonts (e.g. Geist + Geist Mono, or IBM Plex Sans + IBM Plex Mono) preserves the system; swapping the dashed-border/cube vocabulary destroys it. If the type ever reads as generic, the fix is to push the structural signatures harder, not to chase a flashier face.
- **Google-Fonts dependency.** Inter + JetBrains Mono load from a single `<link>`; with no network they fall back to system sans/mono and the deck loses its precision (though the dashed structure survives).
- **The cube graphics are hand-authored SVG, not a component library.** Each cube's face polygons and hatch pattern are written inline; adding cubes means copying and recoloring the polygon set, and odd scales can misalign the hatch pitch (fixed 9px) against the cube size.
- **The graph-paper grid is a fixed 80px pitch.** It is tuned for the 1920×1080 stage; at very different effective scales the cell density can read too busy or too sparse.
- **The noise overlay uses `mix-blend-mode: screen`**, which lightens the charcoal slightly; on surfaces that need a true flat charcoal (e.g. behind a screenshot), the overlay should be reduced or removed locally.
- **Single-accent discipline is fragile under "make it pop" pressure.** Because the icon spectrum (red/blue/green/purple) is already in the palette, it is tempting to promote one to a UI accent — doing so quietly breaks the system. The quarantine (spectrum = cubes/syntax only) must be held deliberately.
- **The dashed border is rendered by the browser's native dash engine**, whose dash length/gap is not tunable per the 1px spec without switching to a border-image; corner rendering of dashes on the 8px radius can vary slightly between engines.
