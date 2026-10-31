# flowbaker

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/flowbaker/flowbaker, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/flowbaker

## Pinned environment

- Project commit: `b0cfbae449e8f7012980110cac75b584d63f68b8`
- Test commit: `b0cfbae449e8f7012980110cac75b584d63f68b8`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 4.2 to 4.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 4.5 | 4.2 | 2 | 2 | [run](https://argusic.com/run/cd84ad7d-cb80-4d5d-89da-ced5c1836163) |

## What was observed on a clean machine

Attempt 1:

- 3.5 min: `Go 1.25 required but not installed in container`
- 0.5 min: `GOPATH not configured`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
