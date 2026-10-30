# zigflow

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/zigflow/zigflow, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/zigflow

## Pinned environment

- Project commit: `1dacad1beb4f5a261aafd4b61e71b43d8409fd39`
- Test commit: `1dacad1beb4f5a261aafd4b61e71b43d8409fd39`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 10 to 10 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2.2 | 10 | 4 | 4 | [run](https://argusic.com/run/530b1cd0-12a1-44d8-bbb4-961eaff75498) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Go 1.27.1 not installed in container`
- 0.5 min: `helm not found (chart tests fail)`
- 0.3 min: `Temporal CLI not found for e2e testing`
- 0.4 min: `Temporal SDK resolves localhost to IPv6 ::1 which fails in this container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
