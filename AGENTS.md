# AGENTS.md

## Purpose

This repository is for academic and research presentations. Use it to create PPTX files, speaker scripts, literature review decks, conference talks, posters, and meeting materials.

Related repositories:

- `Ramblue/research`: shared research materials, source maps, reading queues, datasets, and reusable notes.
- `Ramblue/review`: structured paper reviews, evidence extraction, critique, and talk/poster review.
- `Ramblue/figure`: paper figures, diagrams, visual explanations, Figma assets, and image-generation workflows.
- `Ramblue/writing`: LaTeX manuscript drafting, venue templates, citation integration, strict review loops, and submission preparation.
- `Ramblue/presentation`: meeting decks, literature review decks, conference talks, posters, and speaker scripts.

## Repository Role

Use this repository for:

- meeting decks and progress updates
- literature review presentations
- conference talks
- academic posters
- speaker scripts
- slide outlines
- visual storyboards
- exported PPTX files
- poster-ready layouts

Do not use this repository as the main place for raw literature collection, detailed paper critique, manuscript drafting, or figure source creation. Put those in `Ramblue/research`, `Ramblue/review`, `Ramblue/writing`, and `Ramblue/figure`.

## Presentation Types

### Meeting

Use for lab meetings, advisor updates, project syncs, and internal research discussions.

Default priorities:

- current status
- decisions needed
- blockers
- next actions
- concise evidence

### Literature Review

Use for paper clusters, field maps, method comparisons, and research background presentations.

Default priorities:

- scope and selection criteria
- paper grouping
- method comparison
- evidence quality
- open gaps
- implications for current work

### Conference Talk

Use for formal oral presentations based on a manuscript or project.

Default priorities:

- sharp motivation
- clear contribution
- minimal but convincing method explanation
- result-driven narrative
- memorable takeaways
- timed speaker script

### Poster

Use for poster sessions, visual summaries, and print or digital poster formats.

Default priorities:

- fast visual scanning
- strong title and contribution
- concise method/result blocks
- readable figures
- minimal prose
- clear contact and citation details

## Recommended Structure

- `meeting/`: Internal meeting decks and scripts.
- `literature-review/`: Literature review decks and scripts.
- `conference-talk/`: Conference talks, timed scripts, and slide plans.
- `poster/`: Poster outlines, layouts, and print-ready assets.
- `assets/`: Shared logos, exports, images, and presentation-ready figures.
- `docs/`: Cross-repository workflow and repository documentation.
- `templates/`: Markdown templates for each presentation type.
- `scripts/`: PPTX generation, export, and validation scripts.

## Output Rules

For each substantial presentation project, produce:

- a Markdown planning file
- a slide-by-slide outline
- a speaker script
- a PPTX file when requested
- links to source notes, reviews, figures, or manuscript sections
- unresolved questions or rehearsal notes

When creating PPTX files:

- match the audience and venue
- use figures from `Ramblue/figure` when possible
- avoid text-heavy slides
- keep slide titles meaningful
- preserve citation and source traceability
- verify that text fits and visuals are readable

## Cross-Repository Interaction

Use presentations as the final communication layer.

Prefer relative links when repositories are checked out under the same parent directory:

```md
Source note: ../research/sources/topic-slug/source-slug.md
Review: ../review/reviews/topic-slug/source-slug.md
Figure: ../figure/figures/project-slug/figure-id/spec.md
Manuscript: ../writing/manuscripts/project-slug/main.tex
```

When a presentation makes a substantive claim, link it back to a source note, review, manuscript section, or figure spec.

## Script Rules

- Write scripts in a natural spoken style.
- Keep scripts timed to the intended presentation length.
- Mark optional details separately from required narration.
- Include transitions between slides.
- Do not put the full spoken script onto slides.

## Citation and Evidence Rules

- Do not invent citations, results, or paper claims.
- Use short slide citations where appropriate.
- Keep full citation details in notes or references.
- Distinguish published evidence from internal results or speculative framing.
- For literature review decks, make selection criteria explicit.

## Quality Checklist

Before finishing presentation work, verify:

- target audience and presentation type are clear
- slide purpose is clear for every slide
- script matches the slides
- timing is realistic
- figures are readable
- claims are linked to evidence
- unresolved questions are marked
- PPTX output path is recorded when generated

## Agent Behavior

When acting as an AI presentation agent:

- Build the story before polishing the slides.
- Optimize each deck for its presentation type.
- Use `Ramblue/figure` for figure-heavy work and `Ramblue/writing` for manuscript-derived claims.
- Keep speaker scripts useful for actual delivery.
- Report what was created, what source material it uses, and what still needs rehearsal or review.
