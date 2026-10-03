# tsink

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/aidlx/tsink, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/tsink

## Pinned environment

- Project commit: `277e7449a1df65e2291ecb49820918f7d36ba5d6`
- Test commit: `277e7449a1df65e2291ecb49820918f7d36ba5d6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 6.3 to 28.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 6 | 6.3 | 0 | 0 | [run](https://argusic.com/run/c37e72fd-2a32-4ab7-8cc6-c0e6631f6bb8) |
| 2 | pass | 100 | 27 | 28.7 | 2 | 2 | [run](https://argusic.com/run/d6c8d24f-d3a8-4d43-932f-45e0abf8a095) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `Rust toolchain not found in container`
- `3 flaky tests in tsink-server crate fail in parallel mode (port/race-condition in test harness)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
