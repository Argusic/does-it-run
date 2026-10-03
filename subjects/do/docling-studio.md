# docling-Studio

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/scub-france/docling-Studio, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/docling-studio

## Pinned environment

- Project commit: `e95680a0f0d921a112883091ff078ea13b535e65`
- Test commit: `e95680a0f0d921a112883091ff078ea13b535e65`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 6.9 to 10.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 6.9 | 1 | 1 | [run](https://argusic.com/run/86f3fdef-debd-4a75-ba5b-10c85cacbfea) |
| 2 | pass | 100 | 10 | 10.7 | 1 | 1 | [run](https://argusic.com/run/df83427b-1283-44b2-90d5-41a48ea9e9d7) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node v18.19.1 incompatible with vitest 4.x which requires Node ^20.0.0`

Attempt 2:

- 9 min: `Node.js 18 lacks crypto.hash and File constructor needed by vitest tests`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
