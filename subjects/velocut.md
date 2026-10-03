# velocut

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/open-ribbi/velocut, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/velocut

## Pinned environment

- Project commit: `959857c624f2f150f43adf92263c9a0668f88822`
- Test commit: `959857c624f2f150f43adf92263c9a0668f88822`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 6.6 to 7.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5.5 | 7.4 | 1 | 1 | [run](https://argusic.com/run/e1cb476c-6c58-403c-a79e-7ab7ee823fc4) |
| 2 | pass | 100 | 3 | 6.6 | 0 | 0 | [run](https://argusic.com/run/035b7c21-c623-4dbb-b864-d9017b440e78) |

## What was observed on a clean machine

Attempt 1:

- 1.5 min: `Node.js v18 (system) is too old; project requires >=22.6`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
