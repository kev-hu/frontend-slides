---
version: alpha
name: Twenty SaaS
description: "A refined, high-density SaaS operating-deck system adapted from Twenty.com's CRM interface without copying its landing page. Inter carries the boardroom voice with EB Garamond italic reserved for rare editorial accents such as a large #1 marker, numbered agenda rows, or one emphasized word. The palette is disciplined white/off-white/black with muted gray text, then a small pastel accent set (#DFF7E9, #DFF5FB, #EEE7FF, #FFE8F1, #FFF3C4) used only for artifact boards, status dots, isometric panels, avatars, and product-area cues. The signature move is a presentation-native decision surface: thin deck chrome, oversized thesis typography, artifact boards, agenda rows, three-pillar decision grids, dark stat panels, proof stacks, and rollout roadmaps. CRM UI appears as evidence inside cards and dashboard modules, never as a full landing-page screenshot. Depth comes from 1px borders, 8-16px radii, and quiet two-layer shadows; the register is clean SaaS productivity with enough editorial contrast to feel like an authored deck."

colors:
  background: "#FFFFFF"
  surface: "#FCFCFC"
  surface-alt: "#F9F9F9"
  foreground: "#111111"
  primary: "#1A1A1A"
  muted: "#666666"
  tertiary: "#999999"
  border: "#EDEDED"
  border-subtle: "#F0F0F0"
  pastel-green: "#DFF7E9"
  pastel-cyan: "#DFF5FB"
  pastel-purple: "#EEE7FF"
  pastel-pink: "#FFE8F1"
  pastel-yellow: "#FFF3C4"

typography:
  hero-title:
    fontFamily: "'Inter', sans-serif"
    fontWeight: 600
    fontSize: "clamp(58px, 4.3vw, 82px)"
    lineHeight: 0.96
    letterSpacing: "-0.02em"
    color: "{colors.foreground}"
  section-title:
    fontFamily: "'Inter', sans-serif"
    fontWeight: 600
    fontSize: "clamp(46px, 3.4vw, 64px)"
    lineHeight: 1.02
    letterSpacing: "-0.02em"
    color: "{colors.foreground}"
  content-title:
    fontFamily: "'Inter', sans-serif"
    fontWeight: 600
    fontSize: "clamp(34px, 2.4vw, 46px)"
    lineHeight: 1.06
    letterSpacing: "-0.02em"
    color: "{colors.foreground}"
  card-title:
    fontFamily: "'Inter', sans-serif"
    fontWeight: 600
    fontSize: "clamp(20px, 1.35vw, 26px)"
    lineHeight: 1.22
    letterSpacing: "-0.01em"
    color: "{colors.foreground}"
  body:
    fontFamily: "'Inter', sans-serif"
    fontWeight: 400
    fontSize: "clamp(14px, 0.95vw, 18px)"
    lineHeight: 1.6
    color: "{colors.muted}"
  body-small:
    fontFamily: "'Inter', sans-serif"
    fontWeight: 400
    fontSize: "clamp(11px, 0.75vw, 14px)"
    lineHeight: 1.5
    color: "{colors.muted}"
  label:
    fontFamily: "'Inter', sans-serif"
    fontWeight: 600
    fontSize: "12px"
    lineHeight: 1.4
    color: "{colors.muted}"
  ui-small:
    fontFamily: "'Inter', sans-serif"
    fontWeight: 600
    fontSize: "13px"
    lineHeight: 1.3
    color: "{colors.foreground}"
  mono-key:
    fontFamily: "'Fragment Mono', monospace"
    fontWeight: 400
    fontSize: "12px"
    lineHeight: 1
    color: "{colors.muted}"
  editorial-accent:
    fontFamily: "'EB Garamond', Georgia, serif"
    fontWeight: 600
    fontStyle: italic
    fontSize: "1em"
    lineHeight: 1
    letterSpacing: "-0.01em"
    color: "{colors.foreground}"
  stat-number:
    fontFamily: "'Inter', sans-serif"
    fontWeight: 600
    fontSize: "clamp(112px, 8.6vw, 164px)"
    lineHeight: 0.9
    letterSpacing: "-0.045em"
    color: "{colors.foreground}"
  quote:
    fontFamily: "'Inter', sans-serif"
    fontWeight: 600
    fontSize: "clamp(42px, 3vw, 58px)"
    lineHeight: 1.12
    letterSpacing: "-0.02em"
    color: "{colors.foreground}"

spacing:
  slide-pad: "64px 88px 72px"
  chrome-height: "34px"
  card-padding: "24px"
  component-gap: "16px"
  grid-gap: "22px"
  content-max: "1280px"

canvas:
  width: 100vw
  height: 100vh
  background: "{colors.background}"

components:
  deck-chrome:
    height: "{spacing.chrome-height}"
    borderBottom: "1px solid {colors.border}"
    background: "{colors.background}"
    description: "Thin presentation chrome with logo/section left, context center, page number right; never a website nav bar."
  pill:
    border: "1px solid {colors.border}"
    borderRadius: "999px"
    padding: "0 14px"
    background: "{colors.background}"
    description: "Small rounded metadata chip for status, stars, dates, sections, and filters."
  artifact-board:
    border: "1px solid {colors.border}"
    borderRadius: "16px"
    boxShadow: "0 2px 8px rgba(0,0,0,.04), 0 1px 2px rgba(0,0,0,.06)"
    background: "radial-gradient({colors.border} 1px, transparent 1px) 0 0 / 22px 22px, {colors.surface}"
    description: "Dotted board surface for floating product-evidence cards, not a screenshot frame or website hero."
  dark-stat-panel:
    borderRadius: "18px"
    background: "{colors.foreground}"
    boxShadow: "0 14px 42px rgba(0,0,0,.10), 0 3px 10px rgba(0,0,0,.06)"
    description: "High-contrast metric panel used sparingly for the primary result in an operating review."
  card:
    border: "1px solid {colors.border}"
    borderRadius: "12px"
    boxShadow: "0 2px 8px rgba(0,0,0,.04), 0 1px 2px rgba(0,0,0,.06)"
    background: "{colors.background}"
    description: "Default tweet, metric, task, deal, and feature card container."
  pastel-illustration-panel:
    borderBottom: "1px solid rgba(0,0,0,.06)"
    background: "{colors.pastel-green}"
    texture: "radial halftone dots at 12px spacing"
    description: "Feature-card top panel with pastel background, halftone texture, and simple isometric blocks."
  dotted-field:
    border: "1px solid {colors.border}"
    borderRadius: "12px"
    background: "radial-gradient({colors.border} 1px, transparent 1px) 0 0 / 20px 20px, {colors.surface}"
    description: "Subtle product-canvas field for floating company badges and object maps."
---

## Frontend Slides Fixed-Stage Policy

When this design system is used by the `frontend-slides` skill, generate the final deck as a **fixed 1920×1080 stage** that scales uniformly to the browser viewport. The deck should preserve a 16:9 slide canvas on every screen, including phones; it may letterbox or pillarbox, but it should not reflow slide content for mobile.

This policy has higher priority than any source-template responsive behavior described later in this file. If a later section says the original template is viewport-fluid, treat that as source history only, not as the target generation model for `frontend-slides`.

This policy applies even if values below use `100vw`, `100vh`, `vw`, `vh`, or `clamp()`. Treat those as design proportions to translate into 1920×1080 stage coordinates, not as live responsive rules in the generated deck.

Render each slide at 1920×1080, scale the whole stage with one transform, and verify rendered screenshots for both text overflow and panel overlap.

## Overview

Twenty SaaS translates the feeling of a refined CRM web app into a **boardroom operating deck**, not a product landing page. The system is built around presentation-native artifacts: thin deck chrome, oversized thesis typography, floating evidence cards, numbered agenda rows, three-pillar decision grids, dark stat panels, dashboard tables, customer proof stacks, and rollout roadmaps. CRM UI is a supporting vocabulary inside cards and modules; it should never become a full-page website screenshot or CTA-driven marketing hero.

The type system is deliberately restrained. `{typography.hero-title}`, `{typography.section-title}`, `{typography.content-title}`, and almost every UI element use Inter at 500-700 weight with tight negative tracking. `{typography.editorial-accent}` is EB Garamond italic, used sparingly for inline moments like `#1`, a single emphasized word, or quote punctuation. Do not set full headlines in EB Garamond; the accent only works because the rest of the deck is crisp SaaS UI.

The color system is monochrome-first: `{colors.background}`, `{colors.surface}`, `{colors.surface-alt}`, `{colors.foreground}`, `{colors.muted}`, `{colors.tertiary}`, `{colors.border}`, and `{colors.border-subtle}` do nearly all of the work. Pastels are small and purposeful: `{colors.pastel-green}`, `{colors.pastel-cyan}`, `{colors.pastel-purple}`, `{colors.pastel-pink}`, and `{colors.pastel-yellow}` appear in icon dots, illustrated feature panels, avatars, and object badges. Pastels should never flood a whole deck or become gradients.

Depth comes from `{components.card}`, `{components.artifact-board}`, `{components.dark-stat-panel}`, and `{components.pill}`: 1px borders, small radii, and soft stacked shadows. The deck should feel polished and quiet, never glassy, glossy, neumorphic, cartoonish, or landing-page promotional. Density is medium-high; slides can carry self-contained product diagrams and CRM tables, but every dense element must support a boardroom argument.

Key Characteristics:

- White and off-white SaaS surfaces with thin `{colors.border}` dividers.
- Inter everywhere, EB Garamond italic only as rare editorial accent.
- Thin deck chrome with logo/section, context, and page number; no website navigation or CTA clusters.
- Pill badges for dates, status, filters, GitHub stars, section labels, and sync states.
- Feature tabs with colored dots or small icons in the pastel accent set.
- Agenda rows, decision pillars, stat dashboards, proof stacks, and rollout cards as reusable slide modules.
- Pastel illustrated artifact panels with halftone texture and simple isometric blocks.
- Floating company badges on dotted product fields for ecosystem/object-map slides.
- Soft two-layer shadows; no heavy drop shadows or harsh contrast.
- Medium-high density with scannable hierarchy, not airy marketing whitespace.

## Colors

### Palette

- `{colors.background}` `#FFFFFF`: primary canvas, cards, product shells, pills, and clean content areas. Do not tint the main canvas unless a slide explicitly uses `{colors.surface}` as a product field.
- `{colors.surface}` `#FCFCFC`: secondary panels, lane backgrounds, task surfaces, and app subregions. Use this when a white card needs separation without color.
- `{colors.surface-alt}` `#F9F9F9`: sidebar and subnavigation fields. Keep it slightly darker than `{colors.surface}` so app chrome reads.
- `{colors.foreground}` `#111111`: all main headlines, primary copy, UI labels, and stat numbers.
- `{colors.primary}` `#1A1A1A`: primary button fills, logo marks, selected controls, and dark UI emphasis. Avoid large black blocks except buttons or marks.
- `{colors.muted}` `#666666`: secondary text, body copy, inactive navigation, captions, and long explanations.
- `{colors.tertiary}` `#999999`: disabled text, search placeholders, timestamps, small metadata, and quote marks.
- `{colors.border}` `#EDEDED`: primary 1px borders for cards, shells, dividers, lanes, and pills.
- `{colors.border-subtle}` `#F0F0F0`: internal row dividers and low-emphasis separators.
- `{colors.pastel-green}` `#DFF7E9`: primary illustrated feature background and positive status dot.
- `{colors.pastel-cyan}` `#DFF5FB`: workflow/data accents, secondary isometric block, and avatar gradients.
- `{colors.pastel-purple}` `#EEE7FF`: permissions/model accents, avatar gradients, and object badges.
- `{colors.pastel-pink}` `#FFE8F1`: view/company accents and product tabs.
- `{colors.pastel-yellow}` `#FFF3C4`: task/XP/streak-style accents and warning-neutral badges.

This is a monochrome system with controlled pastel accents, not a multi-color marketing system. Do not add saturated blue/purple gradients, neon accents, or a fifth non-pastel brand color.

### Defaults

- Default slide background: `{colors.background}`.
- Default headline color: `{colors.foreground}`.
- Default body color: `{colors.muted}`.
- Default UI selected state: `{colors.background}` over `{colors.surface-alt}` with `{components.card}` shadow.
- Default border: `1px solid {colors.border}`.
- Default row divider: `1px solid {colors.border-subtle}`.
- Default accent usage: one pastel dot/icon per tab/card, or one pastel illustration panel per content slide.

## Typography

### Font Family Stack

- Inter: the product UI and presentation voice. Use for every headline, body paragraph, card title, table row, label, pill, task, metric, quote, and navigation element.
- EB Garamond italic: editorial accent only. Use for one inline word, `#1`, a quote flourish, or a tiny moment of personality inside an otherwise Inter headline.
- Fragment Mono: keyboard shortcuts and code-like command keys only. Do not use it for broad labels; Inter labels are part of the Twenty feel.

### Typography Scale

| token | size | family | weight | use |
|---|---:|---|---:|---|
| `{typography.hero-title}` | 58-82px | Inter | 600 | Cover and closing headlines; two to three lines max. |
| `{typography.section-title}` | 46-64px | Inter | 600 | Section openers and major argument slides. |
| `{typography.content-title}` | 34-46px | Inter | 600 | Dense content slide headline above grids/cards. |
| `{typography.card-title}` | 20-26px | Inter | 600 | Feature-card titles, panel labels, and major card headings. |
| `{typography.body}` | 14-18px | Inter | 400 | Paragraphs, captions, explanations, and secondary text. |
| `{typography.body-small}` | 11-14px | Inter | 400 | Task descriptions, deal metadata, tweet content, timestamps. |
| `{typography.label}` | 12px | Inter | 600 | Pills, tabs, lane headers, badges, and metadata. |
| `{typography.ui-small}` | 13px | Inter | 600 | Deal titles, compact UI labels, and selected tab text. |
| `{typography.mono-key}` | 12px | Fragment Mono | 400 | Keyboard keys and shortcut glyphs. |
| `{typography.editorial-accent}` | 1em | EB Garamond italic | 600 | Inline accent only; never a full block. |
| `{typography.stat-number}` | 112-164px | Inter | 600 | Big metric slides; tight negative tracking. |
| `{typography.quote}` | 42-58px | Inter | 600 | Quote slide pull text. |

### Defaults

Use `{typography.hero-title}` for the first and last slide. Use `{typography.section-title}` for section openers and thesis slides. Use `{typography.content-title}` above product grids. Use `{typography.card-title}` inside feature cards, task modules, and illustrated cards. Use `{typography.label}` for all chrome. Use `{typography.body}` only after a headline has already established hierarchy.

### Signature Treatments

- Every hero or closing headline may include exactly one `{typography.editorial-accent}` word or phrase. This gives the deck the editorial Twenty-inspired `#1` moment without turning the deck serif.
- Long headlines should use black plus gray line contrast: the first clause in `{colors.foreground}`, the second clause in `{colors.muted}`. This is the main section-heading pattern.
- UI text is small and dense. Pills are 12-13px, lane titles are 12px, deal titles are 13px, and task descriptions are 12px. Enlarging UI text makes the product surfaces feel fake.
- Stat numbers use `{typography.stat-number}` with very tight tracking; supporting metrics stay in compact `{components.card}` tiles.

## Layout

The canvas is a fixed 1920x1080 stage with `{spacing.slide-pad}`. The default persistent chrome is `{components.deck-chrome}`: a 34px row near the top edge with brand/section left, context centered, page number right, and a thin divider underneath. This is deck furniture, not product navigation. Do not add nav links, star badges, login buttons, docs buttons, or CTA clusters.

Layout cycles through six archetypes:

| archetype | composition |
|---|---|
| Cover / hero | Huge thesis headline on the left; `{components.artifact-board}` with floating evidence cards on the right; small metric cards along the bottom. |
| Section / agenda | Oversized argument headline followed by four numbered agenda rows with compact pastel artifact blocks. |
| Content / grid | Three decision pillars, each with a pastel isometric panel, concise argument copy, and checklist rows. |
| Stat / statement | `{components.dark-stat-panel}` for the primary result paired with a dashboard surface, metric cards, and a small table. |
| Quote / proof | Large human quote on the left, proof stack cards on the right; no social-media clutter beyond avatar/name/context. |
| Closing / roadmap | Hero-scale recommendation plus a four-step rollout cadence with week pills. |

Spacing is tight but not cramped. Keep 22px gutters between major content columns, 14-18px gaps inside product grids, 12-14px padding inside small UI cards, and 22-24px padding in larger content cards. Product shell widths can reach 1280px on hero slides; content columns should fit inside a 1744px safe width after slide padding.

Use `{components.artifact-board}` for abstract company/object maps and floating evidence cards. Use `{components.pastel-illustration-panel}` for decision-pillar panels or compact agenda thumbnails. Do not use full-bleed pastel backgrounds; the pastel panels are accents inside the otherwise monochrome system.

## Depth and Elevation

Depth is created by borders, off-white surfaces, and two soft shadow presets. `{components.card}` uses `0 2px 8px rgba(0,0,0,.04), 0 1px 2px rgba(0,0,0,.06)` for default cards. `{components.dark-stat-panel}` uses a larger but still soft lift for the one high-contrast result panel. `{components.artifact-board}` stays quiet so floating cards and thesis type remain the focus.

Use elevation to separate presentation artifacts: floating evidence cards, decision pillars, proof cards, metric tiles, and roadmap rows. Do not shadow every element. Rows, dividers, charts, and dotted fields rely on borders and fills instead.

Avoid heavy modal shadows except for a rare overlay pattern. This template is not glassmorphism and not a dramatic dark SaaS pitch; its credibility comes from quiet product realism.

## Shapes and Treatment

Border radii are restrained: 6px for inputs and keycaps, 8px for buttons/tabs/deal cards, 10px for lanes, 12px for product shells/feature cards/tweet cards, and 999px for pills, avatars, status dots, and company badges. Do not use oversized bubbly rounding.

Border weight is almost always 1px. Use `{colors.border}` for external card boundaries and `{colors.border-subtle}` for internal rows. Selected states use a white surface plus `{components.card}` shadow rather than thick borders.

### Decorative Element Types

- Deck chrome: thin top row with section/context/page number; never website navigation.
- Pastel status dots: 8px circles in the pastel palette, always paired with a tab, sidebar item, or badge.
- Dotted product field: 20px radial dot grid on `{colors.surface}` for company/object maps.
- Floating evidence cards: slightly rotated white cards on a dotted board surface, each with a product-area pill and one argument.
- Isometric blocks: simple skewed rounded rectangles on pastel panels, with one faint offset shadow.
- Halftone texture: radial dots at 12px spacing with low opacity, used only inside pastel illustration panels.
- Keyboard keycaps: 42x34px rounded rectangles in `{colors.surface}` with `{typography.mono-key}`.
- Proof cards: white cards with avatar, name, role/date, and concise operator quote.
- Dark stat panel: one black result panel with giant metric and short interpretation.
- Roadmap rows: tall white action cards with numbered serif marker, owner/action text, and week pill.

## Do's and Don'ts

### Do

- Do make slides feel like boardroom operating artifacts, not product landing pages.
- Do use Inter for nearly everything and EB Garamond italic for one small editorial accent.
- Do keep the monochrome palette dominant and reserve pastels for icons, dots, cards, and illustrations.
- Do use agenda rows, decision pillars, dashboard metrics, proof cards, and rollout rows as content modules.
- Do keep density medium-high with clear gutters, aligned edges, and small UI text.
- Do use soft two-layer shadows only on cards, selected UI, badges, and large product shells.
- Do populate deck chrome with real section labels, dates, page numbers, or context.

### Don't

- Don't clone a marketing website hero, nav bar, CTA row, GitHub stars badge, or product-tour page.
- Don't make full-slide pastel backgrounds or vibrant gradients.
- Don't use EB Garamond for full headlines, body copy, or labels.
- Don't add heavy shadows, glass blur, glossy cards, or dramatic lighting.
- Don't make illustrations single-color blobs or generic stock imagery.
- Don't over-round the UI into a playful consumer-app aesthetic.
- Don't make the deck low-density; this system is for scannable operating detail.
- Don't invent saturated brand colors beyond the controlled pastel set.

## Responsive Behavior

The source inspiration is web-responsive, but frontend-slides output is fixed-stage. Treat all clamp values as proportional guidance that maps into 1920x1080 coordinates. Preserve the 16:9 stage and scale uniformly on smaller screens.

If adapting the system outside frontend-slides, collapse product grids before shrinking typography. On the fixed slide stage, do not reflow: instead reduce the number of modules, shorten copy, or split a dense product surface across multiple slides.

## CJK & International Content

For CJK decks, pair Inter with Noto Sans CJK or Source Han Sans for UI/body text. Preserve the same color, border, and surface grammar, but set letter-spacing to 0 for CJK text and increase line-height by roughly 0.08-0.12 for dense paragraphs.

Do not apply uppercase label styling to CJK strings. Use short label text, full-width punctuation where appropriate, and add 盘古之白 spacing between Latin product names/numbers and CJK characters. EB Garamond italic has no CJK role; omit the editorial accent or replace it with a small Latin numeral/acronym only when it is semantically real.

## Iteration Guide

1. To add a new cover, start with `{components.deck-chrome}`, a huge left-aligned `{typography.hero-title}` thesis, one `{typography.editorial-accent}` accent, a right-side `{components.artifact-board}`, and 2-3 bottom metric cards.
2. To add an agenda slide, use an oversized `{typography.section-title}` and four numbered rows; each row gets one argument, one sentence of explanation, and a compact pastel artifact block.
3. To add a decision slide, create three pillars with pastel illustration panels, concise argument titles, and checklist rows. Avoid web-feature cards and CTA language.
4. To add a metric slide, use `{components.dark-stat-panel}` for one primary result and pair it with dashboard evidence: chart, metric cards, and a small table.
5. To add workflow/process detail, use roadmap rows, task rows, or checklist rows with short labels; do not use sprawling flowcharts.
6. To add customer proof, put the human quote at presentation scale and keep proof cards secondary.
7. To add a closing slide, return to hero typography and pair it with a dated rollout cadence or decision checklist.

## Known Gaps

This template relies on Google Fonts for Inter, EB Garamond, and Fragment Mono. If fonts fail to load, the deck loses the editorial accent and some UI precision. The pillar, dashboard, and roadmap patterns require short labels; verbose deal descriptions or too many table columns should be split across slides. The isometric illustration vocabulary is intentionally simple; complex bespoke diagrams need custom art direction to stay on-system. EB Garamond has no CJK equivalent in this template, so international decks should reduce or remove the editorial accent rather than forcing a mismatched serif.
