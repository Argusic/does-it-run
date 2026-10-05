# SeekStorm

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/SeekStorm/SeekStorm, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/seekstorm

## Pinned environment

- Project commit: `50cb0ddffe1e45eb574f927079d1bcffecf8980b`
- Test commit: `50cb0ddffe1e45eb574f927079d1bcffecf8980b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 62.6 to 62.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 14 | 62.6 | 2 | 2 | [run](https://argusic.com/run/25345b20-ee1e-462c-ac5a-460775bb3827) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `rustc/cargo not found in container; standard install (cargo build) could not start`
- 20 min: `seekstorm_client E2E tests failed 6/7 with HTTP 401 'apikey invalid or missing' and bind failure on port 80 due to stale server`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
