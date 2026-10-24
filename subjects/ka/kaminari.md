# kaminari

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/lucky-chap/kaminari, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/kaminari

## Pinned environment

- Project commit: `a2e666cdf087ff01490b85391b118d6480102d96`
- Test commit: `a2e666cdf087ff01490b85391b118d6480102d96`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 3.5 to 3.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.5 | 3.5 | 1 | 1 | [run](https://argusic.com/run/55ae0b90-d366-493e-9c9c-3f602e1a3ea5) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Missing optional native binding @tailwindcss/oxide-linux-x64-gnu (npm v9 bug on Node 18 fails to install optionalDependencies needed by @tailwindcss/oxide)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
