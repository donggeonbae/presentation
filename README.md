# presentation

Academic and research presentations for the donggeonbae research system.

Use this repository to create meeting decks, literature review decks, conference talks, posters, PPTX files, and speaker scripts.

## Related Repositories

- `donggeonbae/research`: shared source material and reusable research notes.
- `donggeonbae/review`: paper reviews and critique.
- `donggeonbae/figure`: figure generation and visual assets.
- `donggeonbae/writing`: LaTeX manuscript drafting and submission preparation.
- `donggeonbae/presentation`: PPTX, scripts, posters, and talks.

## Presentation Types

- `meeting/`: internal updates and project discussions
- `literature-review/`: paper cluster reviews and field maps
- `conference-talk/`: formal talks based on research contributions
- `poster/`: poster session materials and visual summaries

## Suggested Workflow

1. Choose the presentation type.
2. Start from source notes, reviews, manuscript sections, or figure specs.
3. Create a Markdown planning file from the matching template.
4. Generate or assemble a PPTX when requested.
5. Write a speaker script.
6. Review timing, evidence links, and visual readability.

For paper-review-derived decks, start from `donggeonbae/review/templates/presentation-handoff.md` and preserve the review's logic flow from existing research to limitation, method, results, implications, and remaining gaps.

## Templates

- `templates/meeting.md`
- `templates/literature-review.md`
- `templates/conference-talk.md`
- `templates/poster.md`


## HTML Archive Framework

This repository includes the encrypted static HTML archive framework adapted from `Lukael/research`.

Typical report flow:

```powershell
$env:REPORT_PASSWORD="<local secret>"
node scripts/build-markdown-report.js --slug example-report --input path\to\report.md --title "Example Report"
```

The command creates `projects/<slug>/index.html` and, when `REPORT_PASSWORD` is set, `projects/<slug>/report.enc`. The transient plaintext HTML is written under `build/` and should not be committed.

