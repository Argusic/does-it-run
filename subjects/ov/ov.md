# ov

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/noborus/ov, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/ov

## Pinned environment

- Project commit: `e799baf99eb5b542e1ac835b9b41fde2d6928637`
- Test commit: `e799baf99eb5b542e1ac835b9b41fde2d6928637`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 5.7 to 5.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 6 | 5.7 | 1 | 1 | [run](https://argusic.com/run/e941c78b-fd55-45a8-9033-47cb4dc8c419) |

## What was observed on a clean machine

Attempt 1:

- 6 min: `Go 1.26.0 compiler not found in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
