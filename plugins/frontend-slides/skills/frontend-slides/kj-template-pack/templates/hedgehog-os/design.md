---
version: alpha
name: Hedgehog OS
description: "A charming macOS-inspired glassmorphism system that turns a slide deck into a desktop. The thesis is structural: every content block is a floating frosted-glass app WINDOW with a traffic-light titlebar (red/amber/green dots), a centered Geist Mono filename pill, ~22px rounded corners, and a soft diffuse drop shadow — floating on a warm-beige desktop wallpaper lit by three subtle radial glows (orange top-left, purple top-right, green bottom-center). Recurring OS furniture carries the identity: a glassy menubar with the 9:41 clock, a Finder-style explorer sidebar with an orange-highlighted active row, glass widget cards, a floating AI-coach chat bubble, and a bottom dock. Type is a single OS superfamily — Geist for everything human (display/UI/body, tight negative tracking at large sizes), Geist Mono for everything the machine emits (filename pills, badges, file paths, code snippets, counters). One friendly orange (#F9A526) is the only brand/CTA color; a quarantined status spectrum (green/purple/red/amber) appears only in badges, status dots, traffic lights, and the wallpaper glows. The register is warm, precise, and approachable — light-mode, soft-shadowed, rounded, the deliberate inverse of a flat or brutalist deck."

colors:
  desktop: "#EEEBE4"
  ink: "#1D1B1A"
  muted: "#6B6560"
  accent: "#F9A526"
  accent-deep: "#D9831A"
  sig-red: "#FF5F57"
  sig-amber: "#FEBC2E"
  sig-green: "#28C840"
  info: "#9B8CFF"
  grn: "#2BB673"
  glass: "rgba(255,253,250,0.66)"
  glass-strong: "rgba(255,254,251,0.82)"
  glass-card: "rgba(255,255,255,0.50)"
  hairline: "rgba(29,27,26,0.10)"
  hairline-soft: "rgba(29,27,26,0.06)"
  rim: "rgba(255,255,255,0.65)"

typography:
  eyebrow:
    fontFamily: "'Geist Mono', monospace"
    fontWeight: 500
    fontSize: "14px"
    letterSpacing: "2.5px"
    textTransform: "uppercase"
    color: "{colors.accent-deep}"
  display:
    fontFamily: "'Geist', sans-serif"
    fontWeight: 700
    fontSize: "clamp(64px, 7vw, 96px)"
    lineHeight: 1.02
    letterSpacing: "-0.035em"
    color: "{colors.ink}"
  h1:
    fontFamily: "'Geist', sans-serif"
    fontWeight: 700
    fontSize: "clamp(48px, 5.2vw, 68px)"
    lineHeight: 1.05
    letterSpacing: "-0.03em"
    color: "{colors.ink}"
  h2:
    fontFamily: "'Geist', sans-serif"
    fontWeight: 600
    fontSize: "clamp(30px, 3vw, 40px)"
    lineHeight: 1.12
    letterSpacing: "-0.02em"
    color: "{colors.ink}"
  lead:
    fontFamily: "'Geist', sans-serif"
    fontWeight: 400
    fontSize: "23px"
    lineHeight: 1.5
    color: "{colors.muted}"
  body:
    fontFamily: "'Geist', sans-serif"
    fontWeight: 400
    fontSize: "17px"
    lineHeight: 1.55
    color: "{colors.muted}"
  card-title:
    fontFamily: "'Geist', sans-serif"
    fontWeight: 600
    fontSize: "22px"
    lineHeight: 1.2
    letterSpacing: "-0.01em"
    color: "{colors.ink}"
  quote:
    fontFamily: "'Geist', sans-serif"
    fontWeight: 600
    fontSize: "clamp(32px, 3.4vw, 40px)"
    lineHeight: 1.28
    letterSpacing: "-0.02em"
    color: "{colors.ink}"
  section-numeral:
    fontFamily: "'Geist Mono', monospace"
    fontWeight: 500
    fontSize: "clamp(110px, 12vw, 150px)"
    lineHeight: 0.8
    color: "transparent"
    webkitTextStroke: "2px {colors.ink}"
  stat-num:
    fontFamily: "'Geist', sans-serif"
    fontWeight: 800
    fontSize: "clamp(64px, 7vw, 88px)"
    lineHeight: 0.95
    letterSpacing: "-0.04em"
    color: "{colors.accent-deep}"
  stat-label:
    fontFamily: "'Geist Mono', monospace"
    fontWeight: 400
    fontSize: "14px"
    letterSpacing: "1.5px"
    textTransform: "uppercase"
    color: "{colors.muted}"
  title-pill:
    fontFamily: "'Geist Mono', monospace"
    fontWeight: 400
    fontSize: "13px"
    color: "{colors.muted}"
  exp-item:
    fontFamily: "'Geist', sans-serif"
    fontWeight: 500
    fontSize: "15px"
    color: "{colors.ink}"
  exp-group:
    fontFamily: "'Geist Mono', monospace"
    fontWeight: 400
    fontSize: "11px"
    letterSpacing: "1.5px"
    textTransform: "uppercase"
    color: "{colors.muted}"
  badge:
    fontFamily: "'Geist Mono', monospace"
    fontWeight: 500
    fontSize: "12px"
    color: "{colors.ink}"
  snippet:
    fontFamily: "'Geist Mono', monospace"
    fontWeight: 400
    fontSize: "15px"
    lineHeight: 1.6
    color: "{colors.ink}"
  btn-label:
    fontFamily: "'Geist', sans-serif"
    fontWeight: 600
    fontSize: "17px"
    color: "#FFFFFF"
  btn-ghost:
    fontFamily: "'Geist Mono', monospace"
    fontWeight: 500
    fontSize: "15px"
    color: "{colors.ink}"
  wlabel:
    fontFamily: "'Geist Mono', monospace"
    fontWeight: 400
    fontSize: "11px"
    letterSpacing: "1.5px"
    textTransform: "uppercase"
    color: "{colors.muted}"

spacing:
  menubar-height: "44px"
  titlebar-height: "54px"
  pad-win-body: "46px 52px"
  pad-win-hero: "66px 80px"
  explorer-width: "248px"
  widgets-width: "300px"
  gap-card-grid: "20px"
  pad-card: "28px"
  r-win: "22px"
  r-card: "16px"
  r-pill: "999px"

canvas:
  width: 100vw
  height: 100vh
  background: "{colors.desktop}"

components:
  desktop-wallpaper:
    background: "{colors.desktop} + three radial-gradient glows"
    description: "The slide ground: warm beige (#EEEBE4) overlaid with three soft radial-gradient glows — orange (accent) at 12%/6% top-left, purple (info) at 92%/4% top-right, green (grn) at 50%/108% bottom-center, each ~22-30% alpha fading to transparent by 60%. This is the 'desktop' every window floats on; it is never a flat fill."
  menubar:
    height: "44px"
    background: "rgba(255,253,250,0.55) + backdrop-blur(24px)"
    borderBottom: "1px solid {colors.hairline-soft}"
    description: "Persistent glassmorphic menu bar pinned to the top edge of every slide: a rounded brand logo chip + bold wordmark at left, muted menu words (File/Edit/View/Window/Help), and a right cluster of Geist Mono status text ending in the 9:41 clock. The deck's primary persistent chrome and the strongest 'this is an OS' signal."
  os-window:
    background: "{colors.glass} + backdrop-blur(34px) saturate(1.5)"
    border: "1px solid {colors.hairline}, border-top {colors.rim}"
    borderRadius: "22px"
    boxShadow: "0 40px 90px -30px rgba(29,27,26,0.45), 0 8px 24px -8px rgba(29,27,26,0.18)"
    description: "THE signature. A floating frosted-glass application window that contains nearly all slide content. Translucent near-white fill with a heavy backdrop blur, a 1px hairline border whose TOP edge is a brighter white rim (the glass-highlight), 22px radius, and a soft two-layer diffuse drop shadow. Positioned absolutely on the desktop, sized per archetype. Never square-cornered, never shadowless."
  titlebar:
    height: "54px"
    background: "rgba(255,255,255,0.30)"
    borderBottom: "1px solid {colors.hairline-soft}"
    description: "The top strip of every os-window: three 14px traffic-light dots (red {colors.sig-red} / amber {colors.sig-amber} / green {colors.sig-green}, each with a faint inset rim) at the left, and an absolutely-centered title-pill. The traffic lights are the single most recognizable motif — present on every window, every slide."
  title-pill:
    background: "rgba(255,255,255,0.5)"
    border: "1px solid {colors.hairline-soft}"
    borderRadius: "999px"
    description: "A centered rounded pill in the titlebar holding a small green status dot + a Geist Mono filename (e.g. 'welcome.md — Hedgehog', '~/architecture — Finder', 'Activity Monitor'). Names the window like a real app document; reinforces the filesystem metaphor."
  explorer:
    width: "248px"
    background: "rgba(255,255,255,0.28)"
    borderRight: "1px solid {colors.hairline-soft}"
    description: "Finder-style left navigation rail inside a window. Geist Mono uppercase group headers (SECTIONS, FILES, LIBRARY) over rows of emoji-icon + Geist 500 label. The ACTIVE row is filled with {colors.accent} (white text + orange glow); inactive rows are muted. The system's wayfinding component and the 'explorer-style sidebar' the source vibe asks for."
  glass-card:
    background: "{colors.glass-card} + backdrop-blur(18px)"
    border: "1px solid {colors.hairline}, border-top {colors.rim}"
    borderRadius: "16px"
    boxShadow: "0 14px 30px -16px rgba(29,27,26,0.30)"
    description: "A frosted content tile used in card grids and stat groups. Lighter, smaller-radius echo of the os-window: translucent white fill, hairline+rim border, soft shadow. Holds an icon-tile (rounded 50px white square with an emoji) + card-title + body + a functional badge."
  widget-rail:
    width: "300px"
    background: "rgba(255,255,255,0.16)"
    borderLeft: "1px solid {colors.hairline-soft}"
    description: "Right-hand column of stacked glass widgets (Uptime, Now Playing, Weather) mimicking the macOS Notification Center / desktop widgets. Each widget = Geist Mono uppercase wlabel + a big value or mini-content. Adds density and the third column of the OS three-column grid."
  ai-coach:
    background: "{colors.glass-strong} + backdrop-blur(30px)"
    borderRadius: "20px"
    boxShadow: "0 40px 90px -30px rgba(29,27,26,0.45)"
    description: "A floating frosted chat window (header with gradient avatar + name + ONLINE badge, message bubbles, mono quick-action chips). 'Them' bubbles are white glass with a tail; 'me' bubbles are filled {colors.accent}. The system's most charming accent — a small product touch that signals an assistive, friendly OS. Floats over the desktop near a corner, overlapping nothing critical."
  dock:
    background: "rgba(255,253,250,0.55) + backdrop-blur(24px)"
    border: "1px solid {colors.rim}"
    borderRadius: "22px"
    description: "Bottom-center glass dock holding a row of 52px rounded app icons (emoji on white tiles). Used on cover/closing 'desktop' slides as a footer anchor; optional on content slides. Echoes the window's glass-and-rim treatment."
  badge:
    borderRadius: "999px"
    description: "A small Geist Mono pill with a colored status pip + tinted label. Three quarantined variants: green (rgba(43,182,115,0.14) bg / {colors.grn} text, STABLE/LIVE/HEALTHY), orange (rgba(249,165,38,0.16) / {colors.accent-deep}, CORE/primary), purple (rgba(155,140,255,0.18) / #6f5fd6, ONLINE/NAV/info). The system's functional-metadata vocabulary; every status, count, or tag is a badge."
  snippet:
    background: "rgba(29,27,26,0.05)"
    border: "1px solid {colors.hairline-soft}"
    borderRadius: "10px"
    description: "Inline monospaced code/command panel in Geist Mono with lightly token-colored syntax (keywords purple, strings green, comments muted). The 'monospaced snippet' the source vibe calls for; ties the deck to the technical-product register."
  btn-primary:
    background: "{colors.accent}"
    borderRadius: "13px"
    boxShadow: "0 10px 26px -6px rgba(249,165,38,0.55), 0 2px 6px rgba(249,165,38,0.35)"
    description: "The single high-contrast call to action: solid friendly-orange fill, white Geist 600 label, a → arrow, and a GLOWING orange shadow (the only colored glow on a UI element). One primary button per slide maximum."
  btn-ghost:
    background: "rgba(255,255,255,0.55)"
    border: "1px solid {colors.hairline}"
    borderRadius: "13px"
    description: "Secondary glass button, almost always carrying a Geist Mono shell command ($ brew install …) or a URL. Translucent white with a hairline border; pairs beside the primary button as the 'developer' option."
  section-numeral:
    color: "transparent"
    webkitTextStroke: "2px {colors.ink}"
    description: "A giant outlined (stroke-only) Geist Mono chapter number (01, 02 …) on section-header slides, set beside the section title with the title to its right. The one place type goes hollow — an 'engineering drawing' echo inside the OS frame."
  traffic-lights:
    description: "Three 14px circles — red {colors.sig-red}, amber {colors.sig-amber}, green {colors.sig-green} — at the far left of every titlebar, each with an inset 0.5px dark rim. The deck's universal recognizability anchor; never omitted, never recolored, never reordered."
---

## Frontend Slides Fixed-Stage Policy

When this design system is used by the `frontend-slides` skill, generate the final deck as a **fixed 1920×1080 stage** that scales uniformly to the browser viewport. The deck should preserve a 16:9 slide canvas on every screen, including phones; it may letterbox or pillarbox, but it should not reflow slide content for mobile.

This policy has higher priority than any source-template responsive behavior described later in this file. If a later section says the original template is viewport-fluid, treat that as source history only, not as the target generation model for `frontend-slides`.

This policy applies even if values below use `100vw`, `100vh`, `vw`, `vh`, or `clamp()`. Treat those as design proportions to translate into 1920×1080 stage coordinates, not as live responsive rules in the generated deck.

Render each slide at 1920×1080, scale the whole stage with one transform, and verify rendered screenshots for both text overflow and panel overlap.

## Overview

Hedgehog OS is a **charming macOS-inspired glassmorphism system** — a slide deck dressed as a friendly desktop operating system. Its closest cultural cousins are the macOS Big Sur/Sonoma desktop, the design-system landing pages of Linear and Raycast, and the "windowed product" homepages technical startups use to feel both polished and human. The premise is that a technical deck should feel like a place you recognize: floating app windows on a warm wallpaper, a familiar menubar and dock, an explorer sidebar to keep you oriented — software that is precise without being cold.

The thesis is **structural, not typographic**. The signature move is the **OS window**: nearly every slide's content lives inside a floating frosted-glass application window with a traffic-light titlebar (red/amber/green dots), a centered Geist Mono filename pill, a 22px radius, a 1px hairline border whose top edge brightens to a white glass-rim, and a soft two-layer diffuse drop shadow. Those windows float on a **desktop wallpaper** — warm beige (`{colors.desktop}`) lit by three subtle radial glows (orange top-left, purple top-right, green bottom-center). Around the windows sits the recurring OS furniture: a glassy **menubar** with the canonical 9:41 clock, a Finder-style **explorer sidebar** with an orange-highlighted active row, glass **widget** cards, a floating **AI-coach chat**, and a bottom **dock**. Where the pack's brutalist and Swiss templates reach for hard borders and zero radius, this one reaches for blur, rounding, and a soft shadow — it is their deliberate inverse.

The **type system** is a single OS superfamily in two roles, exactly as an operating system ships one system font. **Geist** (Google Fonts) is the human voice — every display title, section header, body paragraph, card title, and stat figure, with tight negative letter-spacing (−0.02 to −0.04em) at large sizes so headlines set densely and read "Apple-keynote." **Geist Mono** (Google Fonts) is the machine voice — the filename pills, the `// UPPERCASE` eyebrows, the explorer group headers, the badges, the file paths, the shell commands, the code snippets, the stat labels, and the menubar clock. Hierarchy in the prose comes from weight and size (800 stat → 700 display → 600 title → 400 body), not from a second display face; distinctiveness comes from the glass-and-chrome structure, not from an exotic type choice.

The **color philosophy** is one brand accent, strictly held, plus a quarantined status spectrum. Friendly orange (`{colors.accent}` — `#F9A526`) is the only brand color: it fills the one primary CTA (with a glowing orange shadow), highlights the active explorer row, sets the eyebrow (as the darker `{colors.accent-deep}` on light glass), and colors every stat figure. A **status spectrum** — green `{colors.sig-green}`, purple `{colors.info}`, red `{colors.sig-red}`, amber `{colors.sig-amber}` — exists but is quarantined to four jobs only: badge pips/tints, status dots, the titlebar traffic lights, and the wallpaper glows. It never becomes a heading color, a second CTA, or a card fill. The moment a status color sets a headline, the single-accent discipline breaks.

**Depth is soft and atmospheric — the opposite of the pack's flat templates.** Hedgehog leans into translucency and elevation: glass surfaces with `backdrop-filter` blur, a bright top rim that fakes a lit glass edge, and soft diffuse drop shadows that let windows and cards genuinely float over the wallpaper. Corners are generously rounded (22px windows, 16px cards, 13px buttons, pill badges). **Density is medium**: a full content slide can carry an explorer rail + a three-card grid + a code snippet + a three-widget right rail and still breathe, because the window frame and generous radii organize it; statement and quote slides drop to one window with big type and lots of visible wallpaper.

**Key Characteristics:**
- A floating **frosted-glass OS window** with a **traffic-light titlebar** and centered mono filename pill is the signature, present on nearly every slide.
- A **warm-beige desktop wallpaper** lit by **three radial glows** (orange / purple / green) is the ground — never a flat fill.
- A persistent glassmorphic **menubar** (brand + menu words + the **9:41 clock**) anchors the top of every slide.
- A Finder-style **explorer sidebar** with an **orange-highlighted active row** provides wayfinding and the left column of a three-column OS layout.
- **Glass everywhere**: `backdrop-filter` blur + a bright white top **rim** + soft diffuse shadows; nothing is opaque-flat.
- **Geist + Geist Mono** in strict roles: Geist for all prose/display, Geist Mono for every pill, badge, path, snippet, and counter.
- One **friendly orange** (`{colors.accent}`) brand accent with a **glowing CTA shadow**; a green/purple/red/amber spectrum quarantined to badges, dots, traffic lights, and glows.
- **Generously rounded** corners (22 / 16 / 13px, pill badges) and **soft shadows** — the deliberate inverse of flat/brutalist decks.
- Charming product furniture — a floating **AI-coach chat**, glass **widgets**, a bottom **dock** — gives the deck its warm, lived-in personality.
- **Functional badges and mono snippets** everywhere signal a real technical product.

## Colors

### Palette

**Core (committed) palette:**

- **Desktop** (`{colors.desktop}` — `#EEEBE4`): Warm beige. The wallpaper ground beneath the three glows. Never a text color, never a window fill (windows are translucent white glass, not beige).
- **Ink** (`{colors.ink}` — `#1D1B1A`): Deep warm charcoal — not pure black. Every primary headline, card title, body-emphasis, border base, and the section-numeral stroke. The system's text and line color.
- **Muted** (`{colors.muted}` — `#6B6560`): Taupe-grey. Secondary text — leads, body copy, captions, menu words, mono chrome (pills, paths, stat labels, group headers). The system's "quiet" voice.
- **Accent** (`{colors.accent}` — `#F9A526`): Friendly orange. The single brand color — primary CTA fill (+ glowing shadow), active explorer row, the menubar logo chip, the quote mark, badge-orange tint. On light glass, headlines and eyebrows step to **Accent-deep** (`{colors.accent-deep}` — `#D9831A`) for contrast — used for eyebrows and stat figures so the orange stays legible on near-white glass. Never body text; never a card fill behind text.

**Status spectrum — quarantined to badges, dots, traffic lights, and wallpaper glows:**

- **Sig-green** (`{colors.sig-green}` — `#28C840`) / **grn** (`{colors.grn}` — `#2BB673`, the readable badge-text green): success/live status. Traffic-light green, green badge pips, the title-pill status dot, the green wallpaper glow.
- **Info** (`{colors.info}` — `#9B8CFF`): soft purple. Purple badge tint (ONLINE/NAV), the AI-coach avatar gradient, the purple wallpaper glow.
- **Sig-red** (`{colors.sig-red}` — `#FF5F57`) and **Sig-amber** (`{colors.sig-amber}` — `#FEBC2E`): the close/minimize traffic lights. Reserved for the titlebar dots; not used as content color.

**Glass + line tints (derived, not new hues):** `{colors.glass}` (window fill), `{colors.glass-strong}` (AI-coach fill), `{colors.glass-card}` (card fill), `{colors.hairline}` / `{colors.hairline-soft}` (borders and dividers), `{colors.rim}` (the bright white top-edge highlight on glass).

### Defaults

- **Default surface background**: the `{components.desktop-wallpaper}` (warm beige + three radial glows). Content sits inside translucent `{colors.glass}` windows over it. There is no dark-mode surface — the system is light by commitment.
- **Default headline / display color**: `{colors.ink}` on glass. Headlines are never orange (only stat figures and the eyebrow are).
- **Default body / secondary text color**: `{colors.muted}`.
- **Default eyebrow color**: `{colors.accent-deep}` (the darker orange), Geist Mono uppercase, prefixed `//`.
- **Default border / dash color**: `{colors.hairline}` (with `{colors.rim}` on the top edge of glass elements).
- **Default big-number / stat color**: `{colors.accent-deep}`. Every stat figure is orange.
- **Default CTA fill**: `{colors.accent}` with the orange glow shadow.

Commit hard to **one brand accent**. Do not promote a status-spectrum color (green/purple/red) to a heading, a second button, or a card fill. Categorical differentiation comes from badges, the explorer highlight, and the window chrome — never from a new brand hue. There is no dark mode; do not invert to a charcoal ground.

## Typography

### Font Family Stack

The system runs **one superfamily in two faces**, each in a strict, non-overlapping role.

**Geist** (Google Fonts, weights 400/500/600/700/800) is the **human voice** — everything read as language. Display titles and section headers are Geist 700 with tight negative tracking (−0.02 to −0.035em) so large type sets densely and reads like an Apple keynote; stat figures are Geist 800; card titles and buttons are 600; leads and body are 400 in `{colors.muted}`. Geist is never used for a filename pill, a badge, a path, or a code snippet.

**Geist Mono** (Google Fonts, weights 400/500) is the **machine voice** — every signal that the artifact is a piece of software. It sets the `// UPPERCASE` eyebrows (500, 2.5px tracking), the titlebar filename pills, the explorer group headers, the functional badges, the stat labels, the file paths and shell commands in ghost buttons, the inline code snippets (with light syntax coloring), the widget labels, and the menubar clock. Geist Mono is never used for prose.

Because both faces are siblings from one superfamily, the deck reads as coherently "system-designed" as a real OS — the prose↔chrome contrast is carried by face (sans vs mono) and the display hierarchy by weight and size, not by a third face.

### Typography Scale

| Token | Size (clamp / px) | Family | Weight | Use |
|---|---|---|---|---|
| `{typography.display}` | 64–96px | Geist | 700 | Cover/hero headline (tightest tracking, −0.035em) |
| `{typography.stat-num}` | 64–88px | Geist | 800 | Big stat figure, always `{colors.accent-deep}` |
| `{typography.h1}` | 48–68px | Geist | 700 | Section-header and closing headline |
| `{typography.section-numeral}` | 110–150px | Geist Mono | 500 | Giant outlined (stroke-only) chapter numeral |
| `{typography.h2}` | 30–40px | Geist | 600 | Content-slide / statement title above a grid |
| `{typography.quote}` | 32–40px | Geist | 600 | Pull-quote body in a Notes window |
| `{typography.lead}` | 23px | Geist | 400 | Standfirst / subtitle under a headline (muted) |
| `{typography.card-title}` | 22px | Geist | 600 | Glass-card title |
| `{typography.body}` | 17px | Geist | 400 | Card body and paragraph copy (muted) |
| `{typography.btn-label}` | 17px | Geist | 600 | Primary-button label (white) |
| `{typography.btn-ghost}` | 15px | Geist Mono | 500 | Ghost-button shell command / URL |
| `{typography.exp-item}` | 15px | Geist | 500 | Explorer sidebar row label |
| `{typography.snippet}` | 15px | Geist Mono | 400 | Inline code/command snippet (syntax-colored) |
| `{typography.eyebrow}` | 14px | Geist Mono | 500 | `// UPPERCASE` eyebrow, 2.5px tracking, accent-deep |
| `{typography.stat-label}` | 14px | Geist Mono | 400 | Uppercase label under a stat figure |
| `{typography.title-pill}` | 13px | Geist Mono | 400 | Titlebar filename pill (muted) |
| `{typography.badge}` | 12px | Geist Mono | 500 | Functional status/tag badge |
| `{typography.exp-group}` | 11px | Geist Mono | 400 | Explorer group header (SECTIONS / FILES), 1.5px tracking |
| `{typography.wlabel}` | 11px | Geist Mono | 400 | Widget label, uppercase, 1.5px tracking |

### Defaults

- **Default cover headline**: `{typography.display}` (Geist 700, 64–96px, −0.035em), preceded by a `{typography.eyebrow}` mono label.
- **Default section opener**: a `{typography.section-numeral}` outlined numeral beside an `{typography.h1}` title.
- **Default content-slide title**: `{typography.h2}` over a card grid.
- **Default body**: `{typography.body}` (Geist 400, 17px) in `{colors.muted}`; subtitles step up to `{typography.lead}` (23px).
- **Default eyebrow**: `{typography.eyebrow}` — Geist Mono 500, uppercase, 2.5px tracking, always prefixed `//`, in `{colors.accent-deep}`.
- **Default big number**: `{typography.stat-num}` (Geist 800) in `{colors.accent-deep}`.
- **Default mono chrome**: `{typography.title-pill}` / `{typography.badge}` / `{typography.wlabel}` in `{colors.muted}`.

When unsure which display token to reach for, default to `{typography.h2}` for a content-slide opener; reserve `{typography.display}` for the cover and `{typography.section-numeral}` for true section dividers.

### Signature Treatments

These are **non-optional whenever the element type appears**:

- **Every window has a traffic-light titlebar with a centered Geist Mono filename pill.** The three dots (red/amber/green) and the `name.ext — App` pill are the system's universal recognizability anchor; a window without them is just a rounded card.
- **Every eyebrow is Geist Mono, uppercase, 2.5px-tracked, prefixed `//`** (e.g. `// DESIGN SYSTEM · v1.0`). The slash prefix is the system's "comment" signal.
- **Every big stat figure is Geist 800 in `{colors.accent-deep}` (orange)**, with any unit (`%`, `×`) riding smaller in `{colors.muted}` or the same orange. Stats are the only large orange type; a dark stat figure breaks the data signal.
- **Every section-divider numeral is the outlined treatment**: Geist Mono 500, `color: transparent`, `-webkit-text-stroke: 2px {colors.ink}`. A solid-filled numeral collapses the engineering-drawing accent.
- **Display and section headlines carry tight negative tracking** (−0.02 to −0.035em). Geist at default tracking reads generic; the negative tracking is the "set with care" keynote move.
- **Every status, count, or tag is a `{components.badge}`** — a mono pill with a colored pip — not plain text. Badges are the system's metadata vocabulary.
- **Body and headline prose never go mono, and chrome never goes Geist sans.** The Geist-prose ↔ Geist-Mono-chrome split is the identity guardrail.

## Layout

### Canvas System

Each slide is a 1920×1080 stage carrying the `{components.desktop-wallpaper}`. A 44px glass `{components.menubar}` pins to the top edge. The primary content is one (occasionally two) absolutely-positioned `{components.os-window}` floating on the desktop, sized per archetype: a centered ~1180px hero window on the cover, a wide ~1580–1740px window for section/content layouts, a compact ~1060–1200px window for quote/closing. A Geist Mono `NN / NN` counter sits at lower-right. Cover and closing slides add a bottom-center `{components.dock}`.

The **three-column OS grid** appears on the densest content slide: a left `{components.explorer}` rail (≈230–248px), a flexible center content pane, and a right `{components.widget-rail}` (≈300px) — all inside one window. Section slides use explorer + center (two columns); statement/quote slides use a single centered pane.

### Padding and Gap Scale

| Token | Value | Use |
|---|---|---|
| `{spacing.menubar-height}` | 44px | Height of the persistent top menubar |
| `{spacing.titlebar-height}` | 54px | Height of a window's traffic-light titlebar |
| `{spacing.pad-win-body}` | 46px 52px | Default interior padding of a window body |
| `{spacing.pad-win-hero}` | 66px 80px | Roomier padding for hero/cover and closing windows |
| `{spacing.explorer-width}` | 248px | Width of the Finder-style explorer rail |
| `{spacing.widgets-width}` | 300px | Width of the right widget rail |
| `{spacing.gap-card-grid}` | 20px | Gap between glass cards in a grid |
| `{spacing.pad-card}` | 28px | Interior padding of a glass card |
| `{spacing.r-win}` | 22px | Window corner radius |
| `{spacing.r-card}` | 16px | Card / widget corner radius |
| `{spacing.r-pill}` | 999px | Badge / title-pill radius |

### Persistent Chrome

Two elements recur on every slide, plus two on desktop slides:
- **Menubar** (every slide) — brand logo chip + wordmark at left; muted menu words; a right cluster ending in the `9:41 AM` clock. Glassmorphic, blurred, hairline-divided.
- **Counter** (every slide) — `NN / NN` in Geist Mono at lower-right in `{colors.muted}`.
- **Dock** (cover / closing) — a bottom-center glass strip of rounded app icons.
- **Window furniture** (every content window) — the traffic lights + filename pill, which function as the deck's per-slide chrome.

### Surface Variations

The deck cycles through one ground and several window personalities — all light:
- **Desktop wallpaper** (the constant) — beige + three glows, visible around and behind every window.
- **Standard glass window** — the default content container.
- **Explorer window** — a window split into explorer rail + content pane (section, content).
- **Three-column window** — explorer + cards + widget rail (densest content slide).
- **Spotlight/Notes window** — a compact centered window for a quote or a CTA, with lots of wallpaper showing.

There is no surface inversion to dark; "focus" and "statement" moments are achieved by shrinking to a single window with big type and more visible wallpaper, not by flipping to charcoal.

### Signature Compositions

- **Cover (desktop)**: menubar → a centered hero window (eyebrow → two-line `{typography.display}` → lead → orange primary + ghost button + status badge) → a floating `{components.ai-coach}` chat in a corner → optional dock.
- **Section header**: a wide window split explorer | content; outlined `{typography.section-numeral}` beside a multi-line `{typography.h1}`, lead, and a row of badges.
- **Content**: a wide window split explorer | three-card grid + code snippet | widget rail. Each card = icon-tile + `{typography.card-title}` + `{typography.body}` + a badge.
- **Stat**: an "Activity Monitor" window — eyebrow + statement `{typography.h2}` → a 3-up row of glass cards each holding a `{typography.stat-num}` figure + `{typography.stat-label}`.
- **Quote**: a compact "Notes" window centered on the desktop — oversized orange quote mark → `{typography.quote}` → an avatar + attribution row.
- **Closing**: a compact "get-started" window (eyebrow → `{typography.h1}` → orange primary + ghost button → mono contact lines) + a bottom dock.

## Depth and Elevation

### Soft by Commitment

This system is **all about elevation** — the deliberate opposite of the pack's flat templates. Windows, cards, the AI-coach, and the dock genuinely float over the wallpaper. Depth is created four ways:

1. **Translucency + backdrop blur.** Every glass surface uses `backdrop-filter: blur(18–34px) saturate(1.4–1.5)` over a low-alpha near-white fill, so the wallpaper glows bleed faintly through and the surface reads as frosted glass, not paint.

2. **The bright top rim.** Glass elements set `border-top-color: {colors.rim}` (≈65% white) against a darker hairline on the other edges — faking a lit glass edge catching light from above. This is what sells "macOS glass" rather than "translucent rectangle."

3. **Soft diffuse drop shadows.** Windows use a two-layer shadow (`0 40px 90px -30px` ink at 45% + a tighter `0 8px 24px`); cards use a single softer `0 14px 30px -16px`. Shadows are large, soft, and low-opacity — never the hard offset shadows of a brutalist deck.

4. **The orange CTA glow.** The one primary button carries a colored glow shadow (`rgba(249,165,38,0.55)`) — the system's only colored elevation, marking "this is the action."

### Layering Order

Wallpaper (z0) → menubar/dock/counter chrome (z40–50) → windows (floating) → floating AI-coach (above its window). Windows never overlap each other; the AI-coach is the only element allowed to overlap a window edge, and only at a corner.

## Shapes and Treatment

### Border Radius

- **22px** (`{spacing.r-win}`) on os-windows, the AI-coach, and the dock.
- **16px** (`{spacing.r-card}`) on glass cards and widgets; 13px on buttons; 14px on icon-tiles and dock apps.
- **999px** (`{spacing.r-pill}`) on badges and the titlebar filename pill; 50% on traffic lights, status pips, and avatars.

Everything is generously rounded. Hard 0px corners do not exist in this system — square corners immediately collapse the friendly-OS feel into a generic flat deck. (This is the explicit inverse of the pack's brutalist/Swiss templates.)

### Border Weights

- **1px solid `{colors.hairline}`** — the default edge on windows and cards, with the **top edge stepped to `{colors.rim}`** (the glass-highlight).
- **1px solid `{colors.hairline-soft}`** — interior dividers: titlebar bottom rule, explorer/widget rail edges, menubar bottom.
- **inset 0.5px** dark rim on each traffic-light dot.
- No heavy borders, no dashes, no hard outlines. Structure comes from blur, rim, and shadow — not from line weight.

### Decorative Element Types

**OS window** — the floating frosted container with traffic-light titlebar + filename pill. The signature; on nearly every slide.

**Desktop wallpaper** — warm beige + three radial glows (orange/purple/green). The constant ground.

**Menubar** — glass top strip with brand + menu words + 9:41 clock. Persistent chrome.

**Explorer sidebar** — Finder-style file tree with an orange-highlighted active row. Wayfinding + left column.

**Glass card** — frosted content tile (icon-tile + title + body + badge). The grid unit.

**Widget** — small glass tile (uptime / now-playing / weather) in the right rail.

**AI-coach chat** — floating frosted chat with bubbles + mono chips. The charm signal.

**Dock** — bottom-center glass strip of rounded app icons.

**Badge** — mono status pill with a colored pip (green/orange/purple).

**Snippet** — inline mono code/command panel with light syntax coloring.

**Section numeral** — giant outlined (stroke-only) Geist Mono chapter number.

**Traffic lights** — three colored dots; the universal recognizability anchor.

## Do's and Don'ts

### Do

- Put slide content inside a floating `{components.os-window}` with a traffic-light titlebar and a centered Geist Mono filename pill, on the `{components.desktop-wallpaper}` (beige + three glows). The window-on-desktop is the system's identity.
- Keep friendly orange (`{colors.accent}`) as the only brand accent — primary CTA (+ glow), active explorer row, eyebrow (as `{colors.accent-deep}`), and stat figures.
- Use glass everywhere: `backdrop-filter` blur + a bright `{colors.rim}` top edge + soft diffuse shadows. The frosted-with-lit-rim treatment is what reads as macOS.
- Set every eyebrow in Geist Mono, uppercase, 2.5px-tracked, prefixed `//`; set every pill, badge, path, snippet, and counter in Geist Mono too — keep prose in Geist.
- Round generously (22 / 16 / 13px, pill badges) and let windows/cards float with soft shadows.
- Use the Finder-style `{components.explorer}` rail with an orange-highlighted active row for navigation and the left column of the OS grid.
- Quarantine the status spectrum (green/purple/red/amber) to badges, status dots, traffic lights, and wallpaper glows.
- Add charming product furniture — the floating `{components.ai-coach}`, glass `{components.widget-rail}`, the `{components.dock}` — to give the deck its lived-in personality.
- Render big stat figures in Geist 800 orange; render section numerals as outline-only.

### Don't

- Don't square the corners or drop the shadows. Hard 0px corners and flat surfaces collapse the friendly-OS feel — this system is the deliberate inverse of a brutalist deck.
- Don't go dark mode. The system is light-by-commitment; there is no charcoal statement surface. Achieve focus by shrinking to one window with more visible wallpaper.
- Don't promote a status color (green/purple/red) to a headline, a second CTA, or a card fill. One brand accent only.
- Don't omit the traffic lights or the filename pill from a window. They are the recognizability anchor; a window without them is just a card.
- Don't set prose in Geist Mono or chrome in Geist sans. The prose↔mono split is non-negotiable.
- Don't color a headline orange. Only stat figures and the eyebrow are orange; headlines are `{colors.ink}`.
- Don't use a flat beige fill as a window or card surface — surfaces are translucent glass over the wallpaper, never opaque paint.
- Don't drop the `//` on eyebrows or the `$`/`~/` on commands and paths — the terminal punctuation is the system's voice.
- Don't overcrowd a window. The frame and radii organize density, but a statement/quote window should breathe with visible wallpaper around it.
- Don't add heavy borders, dashes, or hard offset shadows. Depth is blur + rim + soft shadow only.

## Responsive Behavior

Hedgehog OS is authored as a **1920×1080 presentation system**. Display type uses `clamp()` with `vw` mid-values; chrome heights, radii, blur radii, border weights, and rail widths are fixed `px`. Per the Fixed-Stage Policy above, `frontend-slides` renders one fixed 1920×1080 stage scaled by a single transform — the notes here are source history, not a generation target.

### Scaling Behavior (source history)
- Display scales 64px → 96px; h1 48px → 68px; h2 30px → 40px; stat figures 64px → 88px; section numerals 110px → 150px.
- Body (17px), lead (23px), and all Geist Mono chrome (11–15px) are fixed.
- Window radii (22px), card radii (16px), rail widths (248/300px), blur radii, and the menubar/titlebar heights are fixed and do not scale.

### Original Desktop Intent
The source macOS-landing language collapsed the three-column grid to one column below ~1050px (explorer becomes a horizontal scroller, the right widget rail drops below the content), and windows widened to fill the viewport on small screens. In `frontend-slides` these do not apply — the deck letterboxes at 16:9 instead of reflowing.

## CJK & International Content

The Latin pairing (Geist / Geist Mono) has clean, well-matched CJK counterparts, so this system localizes well — its identity is structural (windows, glass, traffic lights), which survives a face swap intact. All recommended fonts load via Google Fonts CDN.

### Recommended CJK Pairing

| Role | Latin (default) | CJK counterpart |
|---|---|---|
| Display / headline / card title / stat figure (Geist 600–800) | Geist | 思源黑体 Noto Sans SC 700/900 |
| Body / lead / caption (Geist 400) | Geist | 思源黑体 Noto Sans SC 400 |
| Eyebrow / pill / badge / path / snippet / counter (Geist Mono) | Geist Mono | Latin Geist Mono for ASCII; 更紗黑体 Sarasa Mono SC for any CJK inside a monospace run |

The system is sans-led, so Noto Sans SC carries both display and body (hierarchy comes from weight, size, and the orange accent, exactly as in the Latin original). Sarasa Mono SC preserves the terminal voice when a badge or snippet contains Chinese; pure-ASCII chrome (filename pills like `welcome.md`, `// EYEBROWS`, `$ commands`, `~/paths`, `NN / NN`, the 9:41 clock) stays in Geist Mono.

### Loading

```html
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Geist:wght@400;500;600;700;800&family=Geist+Mono:wght@400;500&family=Noto+Sans+SC:wght@400;500;700;900&display=swap" rel="stylesheet">
```

### Universal CJK Adjustments

- **Line-height**: raise by ~15%. Body 1.7–1.8 (from 1.55), display 1.15–1.25 (from the tight 1.02–1.12). The negative letter-spacing on Latin display must go to 0 for CJK.
- **Letter-spacing**: set to 0 on every CJK run. The −0.02 to −0.035em display tracking and the 1.5–2.5px mono tracking read wrong on square CJK glyphs. Keep tracking only on ASCII chrome that stays in Geist Mono.
- **Text transform**: don't apply `uppercase` to CJK — it has no case. The eyebrow's `//` prefix stays; drop the uppercase transform (keep ASCII portions uppercase if mixed).
- **Punctuation**: use full-width Chinese punctuation （，。：；！？「」） in prose; keep half-width ASCII in snippets, commands, and filename pills.
- **盘古之白**: insert a space between CJK characters and adjacent Latin/digits (write `Hedgehog 窗口系统`, not `Hedgehog窗口系统`).
- **Terminal furniture stays Latin**: filename pills, `//`, `$`, `~/`, and `NN / NN` chrome are part of the OS identity — keep them ASCII even in a CJK deck (a real file is named in ASCII).

### Known CJK Gap

- **Geist Mono's filename-pill / terminal punctuation has no CJK equivalent** and is a strong voice signal; in a CJK build it stays ASCII, producing deliberate Latin/CJK mixing in chrome. This is on-brand (software is named in ASCII) but is a conscious choice.
- **Geist's tight negative tracking is a Latin-only move**; Noto Sans SC at 0 tracking loses a little keynote density. Compensate with weight contrast (900 display vs 400 body) and the orange accent.

## Iteration Guide

1. Any new slide starts with the `{components.desktop-wallpaper}` + the `{components.menubar}` + a `NN / NN` counter, and places content inside one floating `{components.os-window}` with traffic lights + a filename pill.
2. Any new section divider uses an outlined `{typography.section-numeral}` beside an `{typography.h1}` title, inside an explorer-split window; precede the title with a `//` eyebrow.
3. Any new content slide is a window split explorer | center grid | widget rail (drop the widget rail if the content is light). The center holds an `{typography.h2}` title over a row of `{components.glass-card}`s.
4. Any new glass card = icon-tile (rounded white square + emoji) + `{typography.card-title}` + `{typography.body}` + a bottom `{components.badge}`.
5. Any new statistic is `{typography.stat-num}` in `{colors.accent-deep}` with a `{typography.stat-label}` beneath; group 2–4 across glass cards inside an "Activity Monitor" window.
6. Any new CTA pairs the `{components.btn-primary}` (orange, glow, → arrow) with a `{components.btn-ghost}` shell command or URL.
7. Any new eyebrow is Geist Mono uppercase, 2.5px-tracked, `//`-prefixed; any new status/tag/count is a `{components.badge}` with the right pip color.
8. Any new quote uses a compact "Notes" window centered on the desktop: oversized orange quote mark + `{typography.quote}` + avatar/attribution row, with generous visible wallpaper.
9. Any new navigational context uses the `{components.explorer}` rail with the current row highlighted in `{colors.accent}`.
10. If a slide feels flat or monotone, deepen the glass (raise blur / strengthen the rim / soften the shadow) or add a charming widget/AI-coach — never add a second brand color or a dark surface.

## Known Gaps

- **Geist and Geist Mono are clean, neutral faces, not exotic display fonts.** This system's distinctiveness is deliberately structural — the OS window, traffic lights, glass treatment, explorer rail, and single-orange discipline carry the identity, not the type. Swapping the type (e.g. Inter + JetBrains Mono, or SF-adjacent Geist as here) preserves the system; swapping the window/glass vocabulary destroys it. If the type ever reads as generic, push the structural signatures harder rather than chasing a flashier face.
- **`backdrop-filter` is the load-bearing effect.** The frosted-glass look depends on `backdrop-filter: blur()` rendering over the wallpaper. In engines or export paths where `backdrop-filter` is unsupported or disabled, glass surfaces fall back to their flat low-alpha fill and lose much of the depth — verify the render shows true frosting before shipping. (Chromium, used by the render script, supports it.)
- **Google-Fonts dependency.** Geist + Geist Mono load from a single `<link>`; with no network they fall back to system sans/mono and lose the keynote density (the glass structure survives).
- **Light-mode only.** The system commits to a single warm-beige ground and has no dark-surface variant; decks that genuinely need a dark/cinematic statement moment are not served by this template (use a dark template instead). Statement emphasis here is "smaller window, more wallpaper," not surface inversion.
- **Emoji as iconography.** Card icon-tiles, explorer rows, the dock, and widgets use emoji glyphs, which render differently across platforms (Apple vs Noto vs Segoe). For a fully controlled look, swap emoji for a consistent icon set; the layout assumes a single square glyph per tile.
- **The three-column window is the densest the system holds gracefully.** Explorer + three cards + a code snippet + a three-widget rail fills a 1740px window; pushing to four cards or a fourth column overflows. Keep the densest content slide at ≤3 cards + 3 widgets, or widen to two stacked card rows.
- **Glow placement is fixed.** The three wallpaper glows sit at fixed positions (top-left orange, top-right purple, bottom-center green); on windows that fill most of the canvas the glows read only as faint edge tints. That is intentional, but a window larger than ~1740×860 will mask most of the wallpaper personality.
