# phi

**Verdict: runs.** Argusic Score 90 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/pulseaiclub/phi, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/phi

## Pinned environment

- Project commit: `4ca0e30588b2dcd0ac3df98b92a2f6009b21dd55`
- Test commit: `4ca0e30588b2dcd0ac3df98b92a2f6009b21dd55`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 2.4 to 2.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 8 | 2.6 | 1 | 1 | [run](https://argusic.com/run/1d81042a-becb-46e7-ba48-d410abd7e9c5) |
| 2 | pass | 100 | 0 | 2.4 | 1 | 1 | [run](https://argusic.com/run/c6acf256-ba31-4e1b-ac1d-e60bd4a8caad) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go 1.26.3 not installed in container`

Attempt 2:

- `Go 1.26.x not installed in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
