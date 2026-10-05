# go-streams

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/reugn/go-streams, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/go-streams

## Pinned environment

- Project commit: `86444ed50ec3919596ef7bf9e97f69bc5a3fef3d`
- Test commit: `86444ed50ec3919596ef7bf9e97f69bc5a3fef3d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 19.7 to 19.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 15 | 19.7 | 2 | 2 | [run](https://argusic.com/run/089e20ed-eae0-4bc4-886a-2304ea6b132f) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go 1.21+ not installed in container`
- 3 min: `TestBatch and TestBatch_Ptr timing-dependent failures (send on closed channel, wrong batch partitioning) under load`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
