# KJ Template Pack

Kevin's custom template pack for the `frontend-slides` skill. These templates are
selected through `kj-template-pack/selection-index.json`, previewed through each
template's `preview.md`, and fully generated from the selected template's
`design.md`.

## What To Read

1. Read `kj-template-pack/selection-index.json` first.
2. Shortlist candidates from metadata only: `mood`, `tone`, `best_for`,
   `avoid_for`, `formality`, `density`, and `scheme`.
3. For title-slide previews, read only the shortlisted candidate `preview.md`
   files.
4. After the user chooses a KJ template, read exactly that one template's full
   `design.md`.
5. Do not bulk-read every `design.md` in the pack.

## Templates

| Template | Slug | Best fit |
|---|---|---|
| KJ Starter | `kj-starter` | Placeholder starter copied from Blue Professional. |
| Voltcast | `voltcast-brutalist` | Dark brutalist hardware, dev-tools, and technical launches. |
| Redline | `redline` | Swiss/Bauhaus technical reports, strategy decks, and crisp product stories. |
| Duolingo Learn | `duolingo-learn` | Bright gamified education, onboarding, habit, and community decks. |
| Stagehand Dev | `stagehand-dev` | Developer-tools, SDK, API, and technical documentation decks. |
| Hedgehog OS | `hedgehog-os` | Friendly macOS-inspired product, platform, and onboarding decks. |
| Twenty SaaS | `twenty-saas` | Refined high-density SaaS, CRM, workflow, GTM, and product strategy decks. |

## Implementation Contract

`design.md` is the design-system recipe. `preview.md` is only a lightweight
style card for title-slide previews. `reference.html` is retained as proof of
the authored render and is not required for normal generation.

Preview slides must be real title slides for the user's deck. Do not render
template names, option labels, file names, paths, `preview.md`, "generated
from", or user requirement notes on the slide itself.

All templates in this pack target the `frontend-slides` fixed-stage model:
render final decks as a 1920x1080 stage, scale uniformly to the viewport, and
verify screenshots for text overflow and panel overlap.
