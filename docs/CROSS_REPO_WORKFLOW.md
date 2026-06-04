# Cross-Repository Workflow

The donggeonbae research system uses five repositories with distinct roles.

## Repositories

- `donggeonbae/research`: shared source material, research maps, reusable notes, and evidence.
- `donggeonbae/review`: structured paper reviews and comparative critique.
- `donggeonbae/figure`: paper figures, diagrams, visual explanations, Figma assets, and image-generation workflows.
- `donggeonbae/writing`: LaTeX manuscript drafts, venue templates, citation integration, strict review loops, and submission materials.
- `donggeonbae/presentation`: meeting decks, literature review decks, conference talks, posters, and speaker scripts.

## Presentation Flow

1. Pull source context from `research`.
2. Pull critique and paper comparisons from `review`.
3. Pull manuscript claims and venue framing from `writing`.
4. Pull visual assets and figure specs from `figure`.
5. Create the right presentation format in `presentation`.

## Link Convention

```md
Source note: ../research/sources/topic-slug/source-slug.md
Review: ../review/reviews/topic-slug/source-slug.md
Figure: ../figure/figures/project-slug/figure-id/spec.md
Manuscript: ../writing/manuscripts/project-slug/main.tex
Presentation: ../presentation/conference-talk/project-slug/talk.md
```

## Promotion Rules

- A meeting deck can start from current project status and open decisions.
- A literature review deck should start from reviewed papers and comparison tables.
- A conference talk should start from a manuscript argument and figure plan.
- A poster should start from the manuscript contribution and strongest visuals.


