# acebase

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/appy-one/acebase, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/acebase

## Pinned environment

- Project commit: `cf58fb87feee97ff468e33a3ae10c374da5aeeaf`
- Test commit: `cf58fb87feee97ff468e33a3ae10c374da5aeeaf`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 39 to 39 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 39 | 1 | 1 | [run](https://argusic.com/run/6122a336-583c-4ddd-8f7d-f1ef405161e7) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `acebase-core dependency referenced as local file path "file:../acebase-core" which does not exist in this environment`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
