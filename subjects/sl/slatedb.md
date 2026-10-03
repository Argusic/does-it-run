# slatedb

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/slatedb/slatedb, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/slatedb

## Pinned environment

- Project commit: `4478eb907b98c0a52299f359127ccba82c2716b9`
- Test commit: `4478eb907b98c0a52299f359127ccba82c2716b9`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 10.5 to 23.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 10.5 | 0 | 0 | [run](https://argusic.com/run/4fce3768-d676-4171-a1d8-7fe84938f6f7) |
| 2 | pass | 100 | 4 | 23.3 | 1 | 1 | [run](https://argusic.com/run/99bd2e70-d4a1-4a67-9be5-bfaa711c209a) |

## What was observed on a clean machine

Attempt 2:

- 4 min: `Running all 2034 slatedb lib tests in one process is killed by OOM (8 GB container limit)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
