# pitupitu

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/klarluft/pitupitu, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/pitupitu

## Pinned environment

- Project commit: `b8b9487660684b351c8f7e8b8c9c2e5c5f5a21dd`
- Test commit: `b8b9487660684b351c8f7e8b8c9c2e5c5f5a21dd`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 7.8 to 7.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 8 | 7.8 | 3 | 3 | [run](https://argusic.com/run/ac0bd044-7a65-4f50-9526-7c29c24410d2) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `No Rust toolchain in container (cargo: command not found), and no root to apt-install it`
- 0.5 min: `rustup installer rejected --no-profile flag`
- 0.5 min: `Throwaway WebSocket mock cloud failed to compile: tokio 'time' feature missing`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
