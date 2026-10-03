# ratatui

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ratatui/ratatui, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/ratatui

## Pinned environment

- Project commit: `a0189ae4af65f85affef2a4b52bc53551cf50a1d`
- Test commit: `a0189ae4af65f85affef2a4b52bc53551cf50a1d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 3; wall time 7.7 to 9.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 8.6 | 0 | 0 | [run](https://argusic.com/run/8d8a5d0c-8dd5-402d-a3d5-cbcf4ff9563a) |
| 2 | pass | 100 | 7 | 9.1 | 0 | 0 | [run](https://argusic.com/run/8552e3db-b322-4dd4-85a0-0c5bfca31cd6) |
| 3 | pass | 100 | 8 | 7.7 | 1 | 1 | [run](https://argusic.com/run/2a259c5c-6e88-4222-9917-ba7f8c2a5ff9) |

## What was observed on a clean machine

Attempt 3:

- 0.2 min: `Rust toolchain not installed`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
