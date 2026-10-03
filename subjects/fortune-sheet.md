# fortune-sheet

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ruilisi/fortune-sheet, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/fortune-sheet

## Pinned environment

- Project commit: `94346608877db4747406707a177c4b8f3bacdbf9`
- Test commit: `94346608877db4747406707a177c4b8f3bacdbf9`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 3; wall time 5.3 to 6.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.3 | 6.5 | 0 | 0 | [run](https://argusic.com/run/f8f4e006-815c-4737-8715-7de2b9b8f6f7) |
| 2 | pass | 100 | 6 | 6.2 | 1 | 1 | [run](https://argusic.com/run/6b153e87-e4db-4a9c-8f55-aa8f9b56922f) |
| 3 | pass | 100 | 7 | 5.3 | 2 | 2 | [run](https://argusic.com/run/4ad6cf81-cfbd-4b24-9558-0a7a8518a94b) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `postinstall script failed because yarn was not installed`

Attempt 3:

- 1 min: `npm postinstall script used 'yarn run build' but yarn was not on PATH (global install blocked by permissions)`
- 1 min: `Running 'father-build' directly in packages/core failed due to missing format config (the root .fatherrc.js defines cjs/esm formats but packages/core has no .fatherrc.js)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
