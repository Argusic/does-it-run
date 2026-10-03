# jcode

**Verdict: runs.** Argusic Score 80 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/1jehuang/jcode, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/jcode

## Pinned environment

- Project commit: `ff6fb6359af588cd51218dae4d96e7d73968f71d`
- Test commit: `ff6fb6359af588cd51218dae4d96e7d73968f71d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 3; wall time 19.7 to 74.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | n/a | 42.1 | 0 | 0 | [run](https://argusic.com/run/bc50b1cb-ebb4-4acb-853b-915e12df710f) |
| 2 | pass | 90 | 7 | 19.7 | 2 | 1 | [run](https://argusic.com/run/251a0739-8cbb-4a4d-93c0-611540e9a689) |
| 3 | fail | 70 | 31.5 | 74.1 | 4 | 2 | [run](https://argusic.com/run/d4ad2c72-9d9f-4bf7-b9c1-ea2c705eead9) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `Rust toolchain not installed`
- 4 min: `5 pre-existing unit test failures (orcarouter CLI choice missing, provider display name mismatch, auth status report missing Cerebras, followup message content mismatch)`

Attempt 3:

- 0.5 min: `Rust toolchain not installed`
- `1 remaining pre-existing lib test failure: run_auto_poke_followup_targets_below_threshold_todos fails assertion that message contains 'completion confidence'`
- `3 pre-existing e2e session_flow test failures: 'No such file or directory' (session load path issue, exists before my changes)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
