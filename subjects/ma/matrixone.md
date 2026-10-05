# matrixone

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/matrixorigin/matrixone, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/matrixone

## Pinned environment

- Project commit: `7ce783464806490263c184f22aaf5d307225adef`
- Test commit: `7ce783464806490263c184f22aaf5d307225adef`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 33.7 to 33.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 29 | 33.7 | 3 | 3 | [run](https://argusic.com/run/6421bdf3-652c-4b29-842f-d800bc71b2c4) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go 1.26.4+ not installed (system has no go binary)`
- 3 min: `archsimd API mismatch: Load*Slice functions renamed to Load*, Store(&x) must use Store(x[:])`
- 3 min: `Server exited on startup due to stale data directory causing CN admission deadline exceeded`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
