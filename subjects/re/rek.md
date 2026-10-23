# rek

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/lucperkins/rek, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/rek

## Pinned environment

- Project commit: `94ba77be350ce27b9cf3923b878ed57c8dbffed5`
- Test commit: `94ba77be350ce27b9cf3923b878ed57c8dbffed5`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 1.6 to 1.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8 | 1.6 | 1 | 1 | [run](https://argusic.com/run/105edae5-80a1-456e-aa8b-e0a92b8baab4) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Go toolchain missing: go: not found`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
