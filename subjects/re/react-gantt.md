# react-gantt

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/svar-widgets/react-gantt, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/react-gantt

## Pinned environment

- Project commit: `a9d15493dd82330bebe3b2315504ee8fadcf75af`
- Test commit: `a9d15493dd82330bebe3b2315504ee8fadcf75af`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 6.2 to 6.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 6 | 6.2 | 2 | 2 | [run](https://argusic.com/run/abfe1f82-0908-4fba-8dbd-45f0e3bd007f) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Vite 7 requires Node.js 20.19+ (crypto.hash is not a function on Node 18)`
- `xdg-open ENOENT when running vite --open in headless container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
