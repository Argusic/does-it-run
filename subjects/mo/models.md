# models

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/reyamira/models, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/models

## Pinned environment

- Project commit: `80f36dc86838ca791e92d01ca4d3c6ae48b9e991`
- Test commit: `80f36dc86838ca791e92d01ca4d3c6ae48b9e991`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 0.1 to 2.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 0.1 | 0 | 0 | [run](https://argusic.com/run/cfbbdf38-a460-421d-9b8d-caa01c914831) |
| 2 | pass | 100 | 2 | 2.8 | 2 | 2 | [run](https://argusic.com/run/6e2c9158-0365-4239-8b3b-47f173f61806) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `Rust toolchain not installed (rustc, cargo missing)`
- 1 min: `Test failed: aa.json model count 679 outside expected band 450-650`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
