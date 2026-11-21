# reproxy

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/umputun/reproxy, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/reproxy

## Pinned environment

- Project commit: `95539db2008b219588ad8f15ab6da51bc63e09cb`
- Test commit: `95539db2008b219588ad8f15ab6da51bc63e09cb`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 5.1 to 5.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 25 | 5.1 | 0 | 0 | [run](https://argusic.com/run/7aeb1056-dfdc-42a9-99d0-c09fb00985f8) |
| 2 | pass | 100 | 6 | 5.7 | 1 | 1 | [run](https://argusic.com/run/bad796f6-31ba-43f0-bf14-7ec11b18526e) |

## What was observed on a clean machine

Attempt 2:

- 3 min: `Go compiler not installed in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
