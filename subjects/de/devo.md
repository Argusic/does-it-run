# devo

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/7df-lab/devo, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/devo

## Pinned environment

- Project commit: `045d17af7caffb5c50742a6b14119519c65ef0a1`
- Test commit: `045d17af7caffb5c50742a6b14119519c65ef0a1`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 68.7 to 68.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 67 | 68.7 | 1 | 1 | [run](https://argusic.com/run/7343821a-a611-46cd-a30e-05bd2b28498c) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `ACP integration tests (acp_initialization_e2e) timed out because CARGO_BIN_EXE_devo env var was not set, causing test harness to invoke cargo run (slow debug rebuild)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
