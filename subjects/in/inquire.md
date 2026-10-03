# inquire

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/mikaelmello/inquire, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/inquire

## Pinned environment

- Project commit: `3d5b65422a247acc773d767558e34fcb69ab04bf`
- Test commit: `3d5b65422a247acc773d767558e34fcb69ab04bf`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 6.3 to 33.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 6.3 | 0 | 0 | [run](https://argusic.com/run/5cf88b35-d5d4-46bf-baed-4ecfe8bdcd8d) |
| 2 | pass | 100 | 35 | 33.5 | 7 | 7 | [run](https://argusic.com/run/5a3fe5fd-f698-4700-93b6-865da503c5a3) |

## What was observed on a clean machine

Attempt 2:

- 5 min: `Rust toolchain not installed`
- 2 min: `cargo binary missing from rustc install`
- 2 min: `derive_more@2.1.1 requires rustc >= 1.81`
- 3 min: `rust-std component incomplete`
- 10 min: `indexmap@2.13.0 requires rustc >= 1.82 (transitive via rstest)`
- 1 min: `NO_COLOR=1 env var causes crossterm ANSI test failures`
- 3 min: `Disk space exhausted (3 Rust tarballs + build artifacts)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
