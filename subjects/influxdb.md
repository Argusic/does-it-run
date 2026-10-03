# influxdb

**Verdict: could not verify.** Argusic Score 20 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/influxdata/influxdb, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/influxdb

## Pinned environment

- Project commit: `693b1fd1b96cdcb980cf76a1004c0b3f1b46db48`
- Test commit: `693b1fd1b96cdcb980cf76a1004c0b3f1b46db48`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 2; wall time 72.8 to 85.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 85.6 | 0 | 0 | [run](https://argusic.com/run/b7a71490-3fe8-434d-819a-525529547bce) |
| 2 | fail | 20 | n/a | 72.8 | 0 | 0 | [run](https://argusic.com/run/4badc5c4-3a8e-47c4-b73f-8e27ea1d12d7) |

## What was observed on a clean machine

No error was recorded during the valid runs.

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
