# catbus

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/cv-cat/catbus, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/catbus

## Pinned environment

- Project commit: `e637cb43078cbe776313ac3500cf0646c2a7b843`
- Test commit: `e637cb43078cbe776313ac3500cf0646c2a7b843`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 2.7 to 2.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 2 | 2.7 | 1 | 1 | [run](https://argusic.com/run/a83f6edb-e983-4c59-b401-2ceb95666c5e) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `System Node.js is v18.19.1 but catbus requires ^22.22.2 || ^24.15.0 || >=26.0.0`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
