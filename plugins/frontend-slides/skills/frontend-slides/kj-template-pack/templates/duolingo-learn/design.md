---
version: alpha
name: Duolingo Learn
description: "A bright, gamified deck system that abstracts the Duolingo app's visual language into the six canonical slide archetypes. The whole identity rests on Nunito (weights 600/700/800) with one non-negotiable rule — every display headline is lowercase, rounded, and friendly. Feather Green (#58CC02) is the unmistakable hero brand color, supported by a color-psychology accent system: bee yellow (#FFC800) for XP and crowns, fox orange (#FF9600) for streaks, macaw blue (#1CB0F6) for Super/info, cardinal red (#FF4B4B) for hearts/errors, and beetle purple (#CE82FF) as an accent. The signature depth move is the chunky 3D pressable button: a fully-pill-rounded button with a colored bottom shadow (`0 7px 0`) that compresses to `0 3px 0` plus a 4px downward translate when 'pressed'. The second signature is the circular gamified lesson node — a white-ringed gradient-filled disc with a `0 8px 0` bottom shadow and an optional level badge — used as a section-marker and as a node-path motif. Cards are soft 24px-radius rectangles with a faint `0 4px 8px` shadow; progress bars are fully-pill-rounded. NOTHING has sharp corners. The register is playful, energetic, friendly, and intentionally un-corporate; surfaces are bright (white, polar #F7F7F7, and a full-bleed Feather Green panel)."

colors:
  green: "#58CC02"
  green-hover: "#43C000"
  green-mask: "#89E219"
  blue: "#1CB0F6"
  blue-dark: "#1899D6"
  yellow: "#FFC800"
  yellow-dark: "#E5A100"
  orange: "#FF9600"
  orange-dark: "#E08600"
  red: "#FF4B4B"
  red-dark: "#E63F3F"
  purple: "#CE82FF"
  purple-dark: "#B368E0"
  eel: "#4B4B4B"
  wolf: "#777777"
  hare: "#AFAFAF"
  swan: "#E5E5E5"
  white: "#FFFFFF"
  polar: "#F7F7F7"

typography:
  hero-title:
    fontFamily: "'Nunito', sans-serif"
    fontWeight: 800
    fontSize: "clamp(72px, 9vw, 128px)"
    lineHeight: 1.05
    letterSpacing: "-0.02em"
    textTransform: "lowercase"
    color: "{colors.eel}"
  stat-big:
    fontFamily: "'Nunito', sans-serif"
    fontWeight: 800
    fontSize: "clamp(180px, 24vw, 380px)"
    lineHeight: 0.9
    letterSpacing: "-0.02em"
    textTransform: "lowercase"
    color: "{colors.green}"
  section-title:
    fontFamily: "'Nunito', sans-serif"
    fontWeight: 800
    fontSize: "clamp(72px, 7vw, 104px)"
    lineHeight: 1.05
    letterSpacing: "-0.02em"
    textTransform: "lowercase"
    color: "{colors.eel}"
  content-title:
    fontFamily: "'Nunito', sans-serif"
    fontWeight: 800
    fontSize: "clamp(56px, 5vw, 76px)"
    lineHeight: 1.05
    letterSpacing: "-0.02em"
    textTransform: "lowercase"
    color: "{colors.eel}"
  quote:
    fontFamily: "'Nunito', sans-serif"
    fontWeight: 800
    fontSize: "clamp(56px, 6vw, 80px)"
    lineHeight: 1.15
    letterSpacing: "-0.01em"
    color: "{colors.white}"
  card-title:
    fontFamily: "'Nunito', sans-serif"
    fontWeight: 700
    fontSize: "clamp(30px, 2.6vw, 40px)"
    lineHeight: 1.1
    letterSpacing: "-0.01em"
    textTransform: "lowercase"
    color: "{colors.eel}"
  body:
    fontFamily: "'Nunito', sans-serif"
    fontWeight: 600
    fontSize: "clamp(24px, 2vw, 34px)"
    lineHeight: 1.45
    color: "{colors.wolf}"
  body-card:
    fontFamily: "'Nunito', sans-serif"
    fontWeight: 600
    fontSize: "clamp(22px, 1.6vw, 26px)"
    lineHeight: 1.45
    color: "{colors.wolf}"
  button:
    fontFamily: "'Nunito', sans-serif"
    fontWeight: 700
    fontSize: "clamp(20px, 1.6vw, 30px)"
    letterSpacing: "0.03em"
    textTransform: "uppercase"
    color: "{colors.white}"
  pill:
    fontFamily: "'Nunito', sans-serif"
    fontWeight: 800
    fontSize: "clamp(24px, 1.8vw, 30px)"
    letterSpacing: "-0.01em"
    textTransform: "lowercase"
    color: "{colors.eel}"
  eyebrow:
    fontFamily: "'Nunito', sans-serif"
    fontWeight: 800
    fontSize: "clamp(20px, 1.5vw, 28px)"
    letterSpacing: "0.08em"
    textTransform: "uppercase"
    color: "{colors.green}"
  caption:
    fontFamily: "'Nunito', sans-serif"
    fontWeight: 700
    fontSize: "clamp(20px, 1.4vw, 24px)"
    lineHeight: 1.2
    color: "{colors.wolf}"
  node-badge:
    fontFamily: "'Nunito', sans-serif"
    fontWeight: 800
    fontSize: "clamp(16px, 1.1vw, 20px)"
    color: "{colors.eel}"
  counter:
    fontFamily: "'Nunito', sans-serif"
    fontWeight: 800
    fontSize: "22px"
    textTransform: "lowercase"
    color: "{colors.hare}"

spacing:
  pad-slide: "90px 120px"
  pad-card: "40px"
  gap-grid: "40px"
  gap-stat: "24px"
  max-width-content: "1680px"
  node-size: "132px"
  node-size-section: "260px"

canvas:
  width: 100vw
  height: 100vh
  background: "{colors.white}"

components:
  chunky-button:
    background: "{colors.green}"
    color: "{colors.white}"
    borderRadius: "9999px"
    padding: "22px 44px"
    boxShadow: "0 7px 0 {colors.green-hover}"
    pressed: "transform translateY(4px); box-shadow 0 3px 0 {colors.green-hover}"
    description: "THE signature depth move. A fully-pill-rounded uppercase button with a colored solid bottom shadow that reads as 3D thickness. The 'pressed' state compresses the shadow from 0 7px 0 to 0 3px 0 and translates the button down 4px — the button physically depresses. Color variants swap both the fill and the bottom-shadow to a darker shade of the same hue (blue uses blue/blue-dark, etc.)."
  chunky-button-white:
    background: "{colors.white}"
    color: "{colors.green}"
    boxShadow: "0 7px 0 rgba(0,0,0,0.12)"
    description: "White-fill variant of the chunky button for use on the full-bleed green panel and the closing CTA. Green label, neutral dark bottom shadow."
  chunky-button-ghost:
    background: "{colors.white}"
    color: "{colors.blue}"
    border: "3px solid {colors.swan}"
    boxShadow: "0 7px 0 {colors.swan}"
    description: "Secondary 'i already have an account' style button — white fill, 3px swan border, blue label, swan bottom shadow. Pairs beside the green primary on the cover."
  lesson-node:
    size: "132px"
    borderRadius: "50%"
    border: "6px solid {colors.white}"
    background: "linear-gradient(180deg, {colors.green-mask} 0%, {colors.green} 100%)"
    boxShadow: "0 8px 0 rgba(0,0,0,0.15)"
    description: "THE second signature. A circular gamified node: white ring, a top-to-bottom gradient fill, and a 0 8px 0 bottom shadow giving it the same chunky depth as the button. Holds a single emoji glyph (or SVG icon). Color variants: green (default), gold (#FFD93B→yellow, for crown/mastery), blue (Super), purple (accent), and locked (swan fill, grey shadow)."
  node-badge:
    background: "{colors.yellow}"
    color: "{colors.eel}"
    borderRadius: "9999px"
    border: "3px solid {colors.white}"
    description: "Small pill badge clipped to the bottom edge of a lesson node showing a level number or status word ('02', 'done', 'next'). Yellow fill by default; swaps to the node's accent color on non-yellow nodes."
  xp-pill:
    borderRadius: "9999px"
    padding: "14px 28px"
    description: "Fully-rounded stat capsule in the gamification color system — e.g. orange streak (🔥) on #FFF4E0, blue gems (💎) on #E6F6FF, red hearts (❤️) on #FFECEC, yellow XP (💎/⭐) on #FFF8DC. Tinted pastel background + saturated accent text + a leading emoji. Used in the cover stat strip and under stat figures."
  soft-card:
    background: "{colors.white}"
    border: "3px solid {colors.swan}"
    borderRadius: "24px"
    boxShadow: "0 4px 8px rgba(0,0,0,0.06)"
    padding: "40px"
    description: "The content-grid card. A soft 24px-radius rectangle with a 3px swan outline and a faint elevation shadow. The outline color may tint to a pastel of the card's accent (e.g. #FFE2BF for an orange card, #CFEFFF for a blue card)."
  progress-bar:
    background: "{colors.swan}"
    fill: "{colors.green}"
    borderRadius: "9999px"
    height: "28px"
    description: "Fully-pill-rounded progress bar. Swan track, accent-colored fill with an inset 0 -6px 0 rgba(0,0,0,0.06) bottom-rim to echo the chunky depth. Fill color matches the card's accent (green/orange/blue)."
  green-panel:
    background: "{colors.green}"
    color: "{colors.white}"
    description: "Full-bleed Feather Green statement surface. Carries white lowercase display text, white nodes, and the white-fill chunky button. The deck's one inverted surface — used for the quote and (optionally) closing/CTA moments."
  deck-progress:
    height: "12px"
    background: "{colors.green}"
    borderTopRightRadius: "9999px"
    description: "Persistent green progress strip pinned to the bottom-left edge, growing in width with slide index. Pill-rounded on its leading (right) end. Flips to white on the green panel."
  deck-counter:
    color: "{colors.hare}"
    description: "Persistent slide counter 'NN / NN' at bottom-right in Nunito 800 lowercase hare grey. Flips to a light green tint (#DFFFC2) on the green panel."
  node-path:
    description: "A row of lesson nodes connected by short pill-rounded connector bars (green when complete, swan when locked), abstracting the app's winding lesson path into a horizontal progression. Used on the closing slide as a 'you are here' wayfinder."
---

## Frontend Slides Fixed-Stage Policy

When this design system is used by the `frontend-slides` skill, generate the final deck as a **fixed 1920×1080 stage** that scales uniformly to the browser viewport. The deck should preserve a 16:9 slide canvas on every screen, including phones; it may letterbox or pillarbox, but it should not reflow slide content for mobile.

This policy has higher priority than any source-template responsive behavior described later in this file. If a later section says the original template is viewport-fluid, treat that as source history only, not as the target generation model for `frontend-slides`.

This policy applies even if values below use `100vw`, `100vh`, `vw`, `vh`, or `clamp()`. Treat those as design proportions to translate into 1920×1080 stage coordinates, not as live responsive rules in the generated deck.

Render each slide at 1920×1080, scale the whole stage with one transform, and verify rendered screenshots for both text overflow and panel overlap.

## Overview

Duolingo Learn is a **bright gamified deck system** that lifts its visual vocabulary from the Duolingo language-learning app and abstracts it into a slide deck. The premise: a deck should feel like opening the app's home screen — energetic, friendly, rounded, and rewarding — without ever cloning the app's sidebar/topbar/lesson-path chrome onto a slide. Every slide is built from the app's *ingredients* (Feather Green, chunky pressable buttons, circular nodes, XP pills, lowercase rounded type, color-psychology accents) recomposed into the canonical archetypes: cover, section header, content grid, stat, quote, and closing.

The type system is **one face doing every job: Nunito** (Google Fonts, weights 600/700/800). The discipline that makes it read as designed is not face contrast but a single, repeated, non-negotiable rule: **display headlines are always lowercase**, weight 800, with −0.02em tracking. Body and card copy run Nunito 600 in muted Wolf grey. Buttons and eyebrows are the only uppercase moments — short, wide-tracked labels. Because there is just one family, hierarchy comes entirely from weight (600 vs 700 vs 800), size, case, and color. The roundness of Nunito's letterforms is itself a load-bearing brand signal — it is the "friendly, approachable" voice the whole system depends on.

The color philosophy is **one hero plus a labeled accent system**. Feather Green (`{colors.green}` — `#58CC02`) is the unmistakable brand color: every primary button, the logo, the hero stat figure, the deck progress bar, and the one inverted panel. Around it sits a *gamification accent system* where each color carries a fixed meaning: bee yellow (`{colors.yellow}`) = XP / crowns / mastery, fox orange (`{colors.orange}`) = streaks, macaw blue (`{colors.blue}`) = Super / info, cardinal red (`{colors.red}`) = hearts / errors, beetle purple (`{colors.purple}`) = accent. These are not free decoration — they are a semantic palette. Neutrals follow Duolingo's own naming: Eel (`{colors.eel}`) for foreground text, Wolf (`{colors.wolf}`) for muted body, Hare (`{colors.hare}`) for faint chrome, Swan (`{colors.swan}`) for borders, white and Polar (`{colors.polar}`) for surfaces.

Depth is **chunky and physical, never atmospheric**. The system's entire depth language is the *colored bottom shadow*: a solid `0 7px 0` offset under buttons, `0 8px 0` under nodes, that reads as a physical lip of thickness — and on buttons it *compresses* (to `0 3px 0` plus a 4px downward translate) so the button literally depresses when pressed. Cards get a single faint soft shadow (`0 4px 8px rgba(0,0,0,0.06)`) for gentle lift, and progress fills get an inset bottom-rim that echoes the same chunky logic. There are no blurred drop shadows, no glows, no gradients except inside the node discs.

**Density philosophy: medium.** Most slides breathe — a hero is one big lowercase line plus a subhead and two buttons; a stat is one giant green number. The densest the system goes is a three-card content grid, each card a tidy emoji + lowercase title + one body line + a pill progress bar with a numeric callout. The system reads as friendly and confident when it leaves negative space and gamified-but-tidy when it fills a grid; it never goes corporate-dense.

**Key Characteristics:**
- One typeface, Nunito 600/700/800 — hierarchy from weight, size, case, and color, not from multiple faces.
- **Every display headline is lowercase** (weight 800, −0.02em). This is the single most recognizable rule in the system.
- Feather Green (`{colors.green}`) as the one hero color — primary buttons, logo, hero stat, progress bar, the inverted panel.
- A labeled gamification accent system (yellow=XP/crowns, orange=streaks, blue=Super, red=hearts, purple=accent) — colors carry meaning, not just variety.
- The chunky 3D pressable button — pill-rounded, colored `0 7px 0` bottom shadow that compresses to `0 3px 0` + 4px translate on press. THE signature.
- Circular gamified lesson nodes — white-ringed gradient discs with a `0 8px 0` chunky shadow and optional level badge; used as section markers and a horizontal node-path motif.
- XP-style stat pills — fully-rounded pastel-tinted capsules with a leading emoji and saturated accent text.
- Soft 24px-radius cards with a faint `0 4px 8px` shadow and pill-rounded progress bars.
- Gamification emoji motifs throughout: 🔥 streaks, 💎 gems/XP, ❤️ hearts, 👑 crowns, 🦉 the owl, ⭐ stars.
- **Zero sharp corners** — pills at 9999px, cards at 24px, nodes at 50%. Nothing is angular.
- Playful bounce on entry — one orchestrated `cubic-bezier(0.34, 1.56, 0.64, 1)` pop, not scattered micro-interactions.

## Colors

### Palette

- **Green / Feather Green** (`{colors.green}` — `#58CC02`): The hero brand color. Used for the primary chunky button fill, the logo wordmark, the hero stat figure, the deck progress bar, complete node-path connectors, and the one full-bleed inverted panel. This is the color a viewer recognizes the deck by. Never used as body text.
- **Green-hover** (`{colors.green-hover}` — `#43C000`): The darker green used *only* as the bottom shadow of the green chunky button (and its pressed-state shadow). Never a fill or text color on its own.
- **Green-mask** (`{colors.green-mask}` — `#89E219`): The lighter green forming the *top* of the lesson-node gradient (mask-green → feather-green, top to bottom). Node-only.
- **Blue / Macaw** (`{colors.blue}` — `#1CB0F6`): Semantic = Super / info. The ghost-button label, the gems pill text, a blue node, a blue content-card accent + progress fill. `{colors.blue-dark}` (`#1899D6`) is its button bottom-shadow.
- **Yellow / Bee** (`{colors.yellow}` — `#FFC800`): Semantic = XP / crowns / mastery. The gold node fill (with `#FFD93B` as the gradient top), the node level-badge background, the XP pill. `{colors.yellow-dark}` (`#E5A100`) is XP-pill text on cream.
- **Orange / Fox** (`{colors.orange}` — `#FF9600`): Semantic = streaks. The streak pill, an orange content-card accent + progress fill, the 🔥 eyebrow. `{colors.orange-dark}` (`#E08600`) is its button shadow.
- **Red / Cardinal** (`{colors.red}` — `#FF4B4B`): Semantic = hearts / errors. The hearts pill. Use sparingly and only for the hearts/error meaning. `{colors.red-dark}` (`#E63F3F`) is its button shadow.
- **Purple / Beetle** (`{colors.purple}` — `#CE82FF`): Semantic = accent / "next". A purple node and its 'next' badge. The least-used accent; reserve for genuine accent moments. `{colors.purple-dark}` (`#B368E0`) is its button shadow.
- **Eel** (`{colors.eel}` — `#4B4B4B`): Foreground. Every display headline, card title, pill text on light, node-badge number. Not pure black — a warm-neutral dark that keeps the friendly register.
- **Wolf** (`{colors.wolf}` — `#777777`): Muted body text — every paragraph and subhead.
- **Hare** (`{colors.hare}` — `#AFAFAF`): Faint chrome — the slide counter, disabled glyphs.
- **Swan** (`{colors.swan}` — `#E5E5E5`): The universal border / track color — card outlines, progress-bar tracks, ghost-button border, locked-node fill, the letterbox.
- **White** (`{colors.white}` — `#FFFFFF`): Default canvas, node rings, card fills, white-button fill, text on the green panel.
- **Polar** (`{colors.polar}` — `#F7F7F7`): Alternating soft surface — section-header and stat backgrounds. A barely-grey to differentiate surfaces without breaking the bright register.

### Defaults

- **Default surface background**: `{colors.white}`. Alternate to `{colors.polar}` for section-header and stat slides. Switch to a full-bleed `{colors.green}` panel for the quote (and optional CTA) moment.
- **Default headline / display color on light surfaces**: `{colors.eel}`. On the green panel: `{colors.white}`.
- **Default hero stat color**: `{colors.green}` — the giant stat figure is always Feather Green on a light surface.
- **Default body text color**: `{colors.wolf}` on light; `{colors.white}` (or `#DFFFC2` light-green) on the green panel.
- **Default eyebrow color**: the semantically appropriate accent — `{colors.green}` for neutral, `{colors.orange}` for a streak-themed section, etc.
- **Default border / track color**: `{colors.swan}`.
- **Default primary action color**: `{colors.green}` (green chunky button). Secondary action: the ghost button (blue label, swan border).

The system commits to **one hero (green) + a semantic accent set**. Don't introduce a color outside the named palette, and don't use the accents decoratively against their meaning (orange is streaks, red is hearts/errors — don't use red as a generic highlight). Categorical differentiation on a grid comes from the *labeled* accent, not from inventing new hues.

## Typography

### Font Family Stack

The system runs **one face: Nunito** (Google Fonts, weights 600 / 700 / 800), loaded via a single `<link>`. It is a rounded, friendly, geometric-humanist sans — the rounded terminals are the entire "approachable" brand voice. Because there is only one family, the role discipline is enforced by **weight + case + size + color**, not by face contrast:

- **800 (ExtraBold)** — every display headline (hero, section, content title), the hero stat figure, pills, eyebrows, the logo, node badges, the slide counter.
- **700 (Bold)** — card titles, buttons, captions, the quote attribution name.
- **600 (SemiBold)** — all body and card paragraph copy.

The non-negotiable signature is **lowercase display**: every headline and most pills are set `text-transform: lowercase` with −0.02em letter-spacing. The only uppercase moments in the entire deck are buttons and eyebrows (short, wide-tracked, `letter-spacing: 0.03–0.08em`).

### Typography Scale

| Token | Size (clamp) | Family | Weight | Use |
|---|---|---|---|---|
| `{typography.stat-big}` | 180–380px | Nunito | 800 | Hero stat figure — giant lowercase, always `{colors.green}` |
| `{typography.hero-title}` | 72–128px | Nunito | 800 | Cover headline (lowercase) |
| `{typography.section-title}` | 72–104px | Nunito | 800 | Section-header headline (lowercase) |
| `{typography.content-title}` | 56–76px | Nunito | 800 | Content/grid slide headline (lowercase) |
| `{typography.quote}` | 56–80px | Nunito | 800 | Quote body on the green panel (white; quotes keep normal case for the quoted sentence) |
| `{typography.card-title}` | 30–40px | Nunito | 700 | Soft-card title (lowercase) |
| `{typography.body}` | 24–34px | Nunito | 600 | Standard body / subhead (Wolf grey) |
| `{typography.body-card}` | 22–26px | Nunito | 600 | Card body paragraph |
| `{typography.button}` | 20–30px | Nunito | 700 | Chunky-button label (UPPERCASE, +0.03em) |
| `{typography.pill}` | 24–30px | Nunito | 800 | XP / stat pill text (lowercase) |
| `{typography.eyebrow}` | 20–28px | Nunito | 800 | Section eyebrow (UPPERCASE, +0.08em, accent color) |
| `{typography.caption}` | 20–24px | Nunito | 700 | Numeric callout under a progress bar; attribution role line |
| `{typography.node-badge}` | 16–20px | Nunito | 800 | Level / status text inside a node badge |
| `{typography.counter}` | 22px | Nunito | 800 | Persistent slide counter (lowercase, Hare) |

### Defaults

- **Default cover/section headline**: `{typography.hero-title}` / `{typography.section-title}` — lowercase, 800, Eel.
- **Default hero-statistic**: `{typography.stat-big}` — lowercase, 800, `{colors.green}`.
- **Default body**: `{typography.body}` (Nunito 600, Wolf).
- **Default eyebrow**: `{typography.eyebrow}` — uppercase 800 in the section's semantic accent.
- **Default card title**: `{typography.card-title}` (lowercase 700).
- **Default button label**: `{typography.button}` — the only place uppercase pairs with weight 700.
- **Default weight for any display**: 800. Never set a headline below 700.

When unsure which display token to reach for, default to `{typography.content-title}` (56–76px) for a content slide opener and reserve `{typography.stat-big}` for the single big-number moment.

### Signature Treatments

These are **non-optional whenever the element type appears**:

- **Every display headline is lowercase Nunito 800 at −0.02em.** A capitalized or title-case headline immediately breaks the Duolingo identity — lowercase is the system's loudest signal.
- **Every primary action is the chunky 3D button** (`{components.chunky-button}`): pill-rounded, colored `0 7px 0` bottom shadow. A flat button with no bottom shadow is not this system's button.
- **Every eyebrow is uppercase Nunito 800 with +0.08em tracking in a semantic accent color**, usually led by a single emoji (⭐, 🔥, 💎).
- **Hierarchy comes from weight, not from a second face.** Don't import a serif or a mono "for contrast" — the system is mono-family by design.
- **Pills and badges stay lowercase** (except buttons/eyebrows). The friendly lowercase register extends to the gamification chrome.

## Layout

### Canvas System
Each slide targets `100vw × 100vh` (1920×1080 fixed stage). Default slide padding is `{spacing.pad-slide}` (`90px 120px`), with hero/stat/quote slides centering content and dropping explicit padding in favor of a flex-centered column. Content lives within a `{spacing.max-width-content}` (1680px) band.

### Padding and Gap Scale

| Token | Value | Use |
|---|---|---|
| `{spacing.pad-slide}` | 90px 120px | Default slide padding |
| `{spacing.pad-card}` | 40px | Soft-card internal padding |
| `{spacing.gap-grid}` | 40px | Content-grid column gap |
| `{spacing.gap-stat}` | 24px | Gap between XP pills under a stat |
| `{spacing.node-size}` | 132px | Standard lesson-node diameter |
| `{spacing.node-size-section}` | 260px | Oversized section-marker node |

### Persistent Chrome
Two elements appear on every slide:
- **Deck progress bar** (`{components.deck-progress}`) — a 12px-tall `{colors.green}` strip pinned to the bottom-left edge, growing in width with slide index, pill-rounded on its leading end. Flips to white on the green panel.
- **Slide counter** (`{components.deck-counter}`) — `NN / NN` at bottom-right in Nunito 800 lowercase Hare grey. Flips to `#DFFFC2` on the green panel.

### Surface Variations
The deck cycles through three surfaces:
- **White content surfaces** — cover, content grid, closing.
- **Polar (`{colors.polar}`) soft surfaces** — section header, stat. A barely-grey ground that differentiates without dimming the bright register.
- **Full-bleed green panel** — the quote (and optional CTA), white text + white nodes + white-fill button.

### Signature Compositions
- **Cover stat strip**: a top row echoing the app topbar — green logo wordmark left, a cluster of XP pills (🔥 streak / 💎 gems / ❤️ hearts) right — over a centered lowercase hero + subhead + a green button paired with a ghost button.
- **Section node-marker**: an oversized (260px) circular node (often the gold crown) with a level badge, set beside the lowercase section title and an accent eyebrow.
- **Stat statement**: one giant green lowercase figure centered, an accent eyebrow above, a subhead and a row of XP pills below.
- **Node-path closer**: a horizontal row of lesson nodes (done → star → next → locked) joined by short pill connectors, abstracting the app's winding path, above the closing headline + CTA.

## Depth and Elevation

### The Colored Bottom Shadow (the one depth mechanism)
Depth in this system is **physical and chunky, created almost entirely by a solid colored bottom offset** — not a blur:
- **Buttons**: `box-shadow: 0 7px 0 <darker-hue>`. The shadow is the same hue family as the fill, one step darker (green/green-hover, blue/blue-dark, etc.). On press it compresses to `0 3px 0` and the button translates `translateY(4px)` — the lip shrinks and the button sinks. This pressable depression is THE signature interaction.
- **Lesson nodes**: `box-shadow: 0 8px 0 rgba(0,0,0,0.15)` (grey for locked). Same chunky-lip logic, neutral instead of hued.
- **Progress fills**: an `inset 0 -6px 0 rgba(0,0,0,0.06)` bottom-rim, echoing the chunky lip at small scale.

### The Soft Card Shadow
The only *blurred* shadow is a single faint card lift: `0 4px 8px rgba(0,0,0,0.06)`. It gives soft-cards gentle elevation without breaking the flat-and-friendly feel. No card uses a heavier or colored blur.

### No Other Depth
There are no glows, no inner shadows beyond the progress rim, no gradient backgrounds (gradients exist only inside node discs, top-light → bottom-dark of one hue). Surface inversion (the green panel) provides large-scale depth; everything else is the colored-lip language.

## Shapes and Treatment

### Border Radius
**Nothing is sharp.** The radius ladder is fixed:
- **9999px (full pill)** — buttons, XP pills, node badges, progress bars and their fills, deck-progress leading end.
- **50%** — lesson nodes (perfect circles).
- **24px** — soft cards.
- **0px** — does not exist in this system. Even the full-bleed panels are edge-to-edge (no visible corner), so squareness never reads.

Rounded corners are non-negotiable — a sharp corner anywhere collapses the friendly Duolingo register into generic web.

### Border Weights
- **6px solid `{colors.white}`** — the lesson-node ring (10px on the 260px section node).
- **3px solid `{colors.swan}`** — soft-card outline and ghost-button border (may tint to a pastel of the card's accent).
- **3px solid `{colors.white}`** — node-badge ring.
- Borders are always solid and always rounded-following; dashed/dotted do not exist.

### Decorative Element Types

**Chunky 3D button** — pill-rounded, colored bottom shadow, compresses on press. The system's signature. Variants: green primary, white-fill (on green panel / CTA), ghost (swan border + blue label).

**Lesson node** — white-ringed gradient circle with a `0 8px 0` chunky shadow holding one emoji/icon. Variants: green (default), gold (crown/mastery), blue (Super), purple (next/accent), locked (swan + grey shadow). Optional clipped level/status badge.

**XP / stat pill** — fully-rounded pastel-tinted capsule, leading emoji + saturated accent text. The gamification stat chrome.

**Soft card** — 24px-radius, 3px swan (or pastel-accent) outline, faint `0 4px 8px` shadow. Holds emoji + lowercase title + body + a pill progress bar + a colored numeric callout.

**Pill progress bar** — swan track, accent fill with an inset bottom-rim, fully rounded.

**Node path** — a horizontal row of nodes joined by short pill connectors (green=complete, swan=locked) — the winding-path motif made linear.

**Green panel** — full-bleed Feather Green inverted surface for the quote/CTA moment.

## Do's and Don'ts

### Do
- Set every display headline in lowercase Nunito 800 at −0.02em. Lowercase is the system's loudest identity signal.
- Use Feather Green (`{colors.green}`) as the hero — primary button, logo, hero stat, progress bar, the one inverted panel.
- Build every primary action as the chunky 3D button (`{components.chunky-button}`) with its colored `0 7px 0` bottom shadow; show the pressed/compressed state where a "pressed" feel is wanted.
- Use the labeled accent system semantically: yellow=XP/crowns, orange=streaks, blue=Super, red=hearts/errors, purple=accent.
- Use circular lesson nodes (`{components.lesson-node}`) as section markers and as a horizontal node-path on the closer.
- Use XP-style pills (`{components.xp-pill}`) for stats and gamification chrome — pastel tint + saturated text + leading emoji.
- Keep cards soft (24px radius), with the faint `0 4px 8px` shadow and pill-rounded progress bars.
- Use gamification emoji (🔥💎❤️👑🦉⭐) as the icon vocabulary — friendly, on-brand, instantly legible.
- Alternate white and Polar surfaces; reserve the full-bleed green panel for the quote/statement moment.

### Don't
- Don't capitalize or title-case display headlines. Lowercase is non-negotiable.
- Don't use a sharp corner anywhere. Pills are 9999px, cards 24px, nodes 50%.
- Don't add a second typeface (no serif/mono "for contrast") — the system is mono-family Nunito by design.
- Don't make a button flat. The colored bottom shadow that compresses on press is the system's signature; a shadowless button is off-system.
- Don't use the accent colors against their meaning (red is hearts/errors, orange is streaks — not generic highlights).
- Don't introduce a color outside the named palette.
- Don't go corporate-dense or muted/desaturated — keep it bright, playful, and breathing.
- Don't use blurred/colored drop shadows beyond the single faint card lift; depth is the chunky colored lip.
- Don't render the app's literal sidebar/topbar/lesson-path layout onto a slide — abstract the vocabulary into the deck archetypes.

## Responsive Behavior

Duolingo Learn is authored as a **fixed 1920×1080 presentation system**. The reference uses fixed px throughout; the frontmatter expresses sizes as `clamp()` proportions so a generator can translate them into stage coordinates. The fixed-stage policy above governs final output regardless of any source-fluid notes.

### Scaling Behavior
- Hero stat scales 180px → 380px on viewport width.
- Headlines scale 56px → 128px depending on archetype.
- Body scales 22px → 34px.
- Node diameters, border weights (6px ring, 3px outlines), and the chunky bottom-shadow offsets (`0 7px 0`, `0 8px 0`) are fixed and do not scale.

### Mobile
The source app was responsive (the original HTML used `auto-fit` grids and flex stacking), but for `frontend-slides` the deck renders fixed-stage and letterboxes rather than reflowing. Treat the source's responsive grid behavior as history only.

### Interactive States
- The chunky button compresses (`0 7px 0` → `0 3px 0`, `translateY(4px)`) on hover/press — the deck may render either the rest or pressed state per slide.
- Lesson nodes scale `1.08` on hover via the bounce easing (`cubic-bezier(0.34, 1.56, 0.64, 1)`); screenshots capture the settled state.
- Entry: one orchestrated staggered `pop` (opacity + translateY(34px) + scale(0.96→1)) on the same bounce easing; `--d` staggers reveals. Celebration-pop variant runs 0.4s same easing.

## CJK & International Content

The system is friendly-rounded and translates to CJK by swapping Nunito for a rounded CJK family; all recommended fonts load via CDN.

### Recommended CJK Pairing

| Role | Latin (default) | CJK counterpart |
|---|---|---|
| Display / hero / stat / section / card titles (lowercase 800) | Nunito 800 | 站酷快乐体 ZCOOL KuaiLe, or Noto Sans SC 900 / 黑体-rounded |
| Body / card body (600) | Nunito 600 | Noto Sans SC 500 |
| Buttons / eyebrows (uppercase) | Nunito 700/800 | Noto Sans SC 700 (no transform) |

ZCOOL KuaiLe is a rounded, playful Chinese display face that best preserves Nunito's friendly roundness; Noto Sans SC is the dependable fallback for coverage.

### Universal CJK Adjustments
- **Lowercase doesn't apply to CJK** (CJK has no case). The "lowercase headline" signature becomes "rounded, casual, single-weight-heavy headline." Lean harder on the *rounded face* + green + node motifs to carry the playful register the lowercase rule carried in Latin.
- **Letter-spacing**: set to 0 on every CJK run; the −0.02em display tracking and the +0.08em eyebrow tracking both read as gappy on square glyphs.
- **Text-transform**: remove `uppercase` from buttons/eyebrows for CJK runs.
- **Line-height**: open display from ~1.05 to ~1.2, body to ~1.6.
- **Punctuation**: use full-width Chinese punctuation （，。！？「」）.
- **盘古之白**: insert an ASCII space between CJK characters and adjacent Latin/digits (e.g. `+312% 周活跃`).
- **One font per sentence**: let the chosen CJK face handle mixed CJK+Latin in a unified rounded style.

## Iteration Guide

1. Any new content slide opens with a `{typography.content-title}` lowercase headline, optionally preceded by a `{typography.eyebrow}` in a semantic accent.
2. Any new statistic is `{typography.stat-big}` in `{colors.green}`, optionally with `{components.xp-pill}` capsules below.
3. Any new body paragraph is `{typography.body}` (Nunito 600) in `{colors.wolf}`.
4. Any new primary action is `{components.chunky-button}` (green); a secondary action is the ghost variant; on the green panel use the white variant.
5. Any new card uses `{components.soft-card}` (24px radius, faint shadow), holding an emoji + lowercase `{typography.card-title}` + `{typography.body-card}` + a `{components.progress-bar}` + a colored numeric `{typography.caption}`.
6. Any new section header pairs an oversized `{components.lesson-node}` (260px, often the gold crown with a badge) beside the lowercase `{typography.section-title}`.
7. Any new quote/statement uses the full-bleed `{components.green-panel}` with white `{typography.quote}` text and a node-avatar attribution.
8. Any new closing uses a `{components.node-path}` row above the headline + a `{components.chunky-button}` CTA.
9. To color-code a grid, assign each card a semantic accent (green/orange/blue) and carry it consistently through the card's border tint, progress fill, and numeric callout.
10. If a slide feels monotone, switch the surface (white → Polar → green panel) — don't add an off-palette color or a second typeface.

## Known Gaps

- **Mono-family by design.** The entire system is Nunito; there is no second face for contrast, so all hierarchy rests on weight/size/case/color. If Nunito fails to load, the deck collapses to a generic system sans and loses its identity entirely (Google Fonts dependency).
- **The lowercase-headline signature does not survive CJK** (CJK has no case). CJK builds must lean on the rounded face + green + node motifs to carry the playful register; the deck reads slightly less distinctively "Duolingo" in CJK.
- **The accent system is semantic, which constrains free color use.** Because orange=streaks and red=hearts/errors carry fixed meaning, a generator can't grab them as neutral highlight colors without implying that meaning — green/blue/yellow are the safer general-purpose accents.
- **The chunky bottom-shadow offsets are fixed px** (`0 7px 0` buttons, `0 8px 0` nodes). At extreme stage scales the lip may look slightly thin or thick relative to type; it's tuned for the 1920×1080 stage.
- **The node-path closer assumes ≤ ~6 nodes** fit one row at 132px + connectors within the content band; longer paths would need a smaller node size or a second row.
- **Emoji rendering varies by platform.** The gamification icons (🔥💎❤️👑🦉) render as the host OS's emoji set; the reference shows Apple glyphs. For pixel-consistent output across machines, swap to inline SVG icons in the same shapes.
