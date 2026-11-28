# examples

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/chromedp/examples, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/run/8abd75fe-024c-4a3d-8ebe-8cd07b2793b5

## Pinned environment

- Project commit: `d25ef08a50326a3f6de61f157e3abee69c898d03`
- Test commit: `d25ef08a50326a3f6de61f157e3abee69c898d03`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 6.1 to 6.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 6 | 6.1 | 3 | 3 | [run](https://argusic.com/run/8abd75fe-024c-4a3d-8ebe-8cd07b2793b5) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go 1.27 not installed in container`
- 3 min: `Chrome not installed in container`
- 1 min: `Chrome sandbox fails for non-root user (uid 1001)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
