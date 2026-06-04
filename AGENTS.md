# AGENTS.md

## Purpose

This repository is for academic and research presentations. Use it to create PPTX files, speaker scripts, literature review decks, conference talks, posters, and meeting materials.

Related repositories:

- `donggeonbae/research`: shared research materials, source maps, reading queues, datasets, and reusable notes.
- `donggeonbae/review`: structured paper reviews, evidence extraction, critique, and talk/poster review.
- `donggeonbae/figure`: paper figures, diagrams, visual explanations, Figma assets, and image-generation workflows.
- `donggeonbae/writing`: LaTeX manuscript drafting, venue templates, citation integration, strict review loops, and submission preparation.
- `donggeonbae/presentation`: meeting decks, literature review decks, conference talks, posters, and speaker scripts.

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

Do not use this repository as the main place for raw literature collection, detailed paper critique, manuscript drafting, or figure source creation. Put those in `donggeonbae/research`, `donggeonbae/review`, `donggeonbae/writing`, and `donggeonbae/figure`.

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
- review handoff from `donggeonbae/review` when available
- paper grouping
- figure snapshots that explain the paper's logic
- prior limitation to method to result to implication narrative
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

When the source is a review report from `donggeonbae/review`, preserve the review's logic flow:

```text
existing research -> limitation -> method -> result -> result implication -> remaining limitation -> broader implication
```

Use the review's figure snapshots as primary slide visuals whenever they clarify the argument.

When creating PPTX files:

- match the audience and venue
- use figures from `donggeonbae/figure` when possible
- use figure snapshots from `donggeonbae/review` when the deck is based on a paper review
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
- review-derived decks preserve the paper's logical flow
- claims are linked to evidence
- unresolved questions are marked
- PPTX output path is recorded when generated

## Static HTML Archive Framework

This repository follows the source-derived encrypted static HTML archive pattern adapted from `Lukael/research`.

Framework files:

- `index.html`: public archive index.
- `styles/site.css`: shared dark archive styling.
- `scripts/site.js`: discovers `projects/<slug>/` folders through the GitHub Contents API or local directory listing.
- `scripts/decrypt-report.js`: unlocks `projects/<slug>/report.enc` in the browser using Web Crypto.
- `scripts/encrypt-report.js`: encrypts plaintext HTML into `report.enc` using `REPORT_PASSWORD`.
- `scripts/build-markdown-report.js`: builds a project unlock shell and optional encrypted report from Markdown.
- `scripts/build-3dgs-ri-report.js`: source-derived example builder kept for reference; prefer `build-markdown-report.js` for new work.
- `templates/unlock-template.html`: public password unlock shell.
- `templates/report-template.html`: dark two-column encrypted report body template.
- `projects/<slug>/`: public unlock shell plus encrypted payload for each protected report.

Do not commit plaintext protected report bodies under `projects/`. Use `build/` for transient plaintext output and keep encrypted payloads in `projects/<slug>/report.enc` when a report should be published.
## Agent Behavior

When acting as an AI presentation agent:

- Build the story before polishing the slides.
- Optimize each deck for its presentation type.
- When working from a review handoff, preserve the review's evidence chain and strongest figure snapshots.
- Use `donggeonbae/figure` for figure-heavy work and `donggeonbae/writing` for manuscript-derived claims.
- Keep speaker scripts useful for actual delivery.
- Report what was created, what source material it uses, and what still needs rehearsal or review.



