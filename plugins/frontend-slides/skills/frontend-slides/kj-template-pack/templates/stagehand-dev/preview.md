# Stagehand Dev Preview Card

Use this small file for title-slide previews only. For final deck generation, read the full design doc listed below.

## Files

- Full design doc: `kj-template-pack/templates/stagehand-dev/design.md`
- Preview card: `kj-template-pack/templates/stagehand-dev/preview.md`

## Selection Metadata

- Slug: `stagehand-dev`
- Tagline: Developer-tools landing-page system — dashed-border graph-paper grid, one golden-yellow accent, and isometric hatched cubes.
- Mood: technical, precise, structured, under-decorated
- Tone: engineered, confident, documentation-grade, dev-native
- Formality: medium
- Density: medium
- Scheme: mixed
- Best for: SDK launches, dev-tool and API pitches, technical documentation decks, open-source project intros, infra/platform overviews, engineering all-hands. Also a strong, unexpected pick for a fintech or data-product deck that wants to read as rigorous and built rather than glossy — anywhere a "made by engineers" register beats marketing polish.
- Avoid for: warm, emotional, or consumer-lifestyle decks; brand/creative storytelling that wants big imagery or expressive type. The flat, technical, single-accent register reads as cold for those.

## Visual Snapshot

A developer-tools presentation system — the visual language of a modern SDK or open-source product deck (Vercel, Railway, Browserbase's Stagehand) brought to slides. The thesis is structural, not typographic: a 1px **dashed border** is the signature, applied as a full system — a dashed rectangle insets 56px from every slide edge, a faint 80px graph-paper grid underlays cream surfaces, and every card, divider, secondary button, and code block is ruled in dashes rather than solid lines or drop shadows. The single brand accent is a golden yellow (#F5A623): it fills the one primary CTA, colors the `// UPPERCASE` mono eyebrows, and drives every big stat figure. A secondary red/blue/green/purple spectrum is quarantined to the isometric 3D cube graphics — hand-built SVG cubes with a diagonal line-hatched right face, the system's only illustration.

Type is the authentic dev pairing: Inter (600 display, 400 body) for everything human-readable, JetBrains Mono for every label, breadcrumb, shell command, code block, stat, and chrome detail — the mono carries a "terminal voice" (`// eyebrows`, `~/breadcrumbs`, `$ commands`, `NN / NN` counters). Surfaces alternate between warm cream (#F7F4EF) content slides and charcoal (#1F1F1F) statement sections carrying an feTurbulence noise texture and dashed-light borders. The register is flat and precise: square-ish radii (8px frames/cards, 4px buttons), zero shadows, zero gradients.

## Preview Ingredients

- Palette: bg cream #F7F4EF; dark charcoal #1F1F1F; card white #FFFFFF; ink #1A1A1A; primary golden-yellow #F5A623 (only accent); cube spectrum red #E74C3C / blue #3498DB / green #27AE60 / purple #9B59B6 (cubes only)
- Typography: Inter (600 display / 400 body) + JetBrains Mono (all labels, chrome, code). See full design doc after selection.
- Signature move: 1px DASHED border as a full system — 56px-inset slide frame + 80px graph-paper grid underlay + dashed cards, dividers, buttons, and code blocks. No shadows, no gradients.
- Signature move: Single golden-yellow accent (#F5A623) — primary CTA fill, mono eyebrows, big stat figures; never a second UI color.
- Signature move: Isometric 3D cubes drawn as SVG with a 45° line-hatched right face; the red/blue/green/purple spectrum lives ONLY inside them.
- Signature move: Inter-prose ↔ JetBrains-Mono-chrome split, with terminal punctuation (`//`, `$`, `~/`, `NN / NN`) as the dev-tool voice.
- Signature move: Cream-content ↔ noisy-charcoal-statement surface alternation; dark surfaces carry feTurbulence film-grain and switch borders to dashed-light.

## International / CJK Preview Note

- This sans-led system localizes cleanly: swap Inter for Noto Sans SC (hierarchy by weight + the yellow accent), keep ASCII terminal chrome (`//`, `$`, `~/`) in JetBrains Mono.
- For CJK runs, set letter-spacing to 0, loosen line-height ~15%, and drop uppercase transforms. Use the full `design.md` CJK section after selection.

## Preview Rules

- Build exactly one title slide at 1920x1080 inside the fixed-stage model.
- Preserve the palette, type roles, surface rhythm, and decorative vocabulary described above.
- Use the user's real title/subtitle/context; do not copy demo slide content.
- The rendered preview must look like a real first slide, not a template-selection card.
- Never place internal workflow text on the slide: no `preview`, `generated from`, `preview.md`, `template`, `preset`, `style option`, `Option A/B/C`, file names, paths, or source-doc labels.
- Never place the template name or slug on the slide itself; mention it only in the chat message.
- Never place user requirement notes such as desired vibe, audience, or internal-use labels on the slide unless the user explicitly wants those exact words in the deck.
- Use only real deck content for visible chrome: deck title, real section title, date, author, company, page number, or genuine content phrases from the user material.
- Do not read `reference.html` for preview generation.
- Do not read other templates' `design.md` files.
- After the user picks this template for the full deck, read the full design doc before generating final slides.
