# FutureSDR

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/FutureSDR/FutureSDR, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/futuresdr

## Pinned environment

- Project commit: `729f7aeba9fc47a5f5d8a2c88568ef78f6f868a8`
- Test commit: `729f7aeba9fc47a5f5d8a2c88568ef78f6f868a8`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 14.8 to 14.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 35 | 14.8 | 4 | 4 | [run](https://argusic.com/run/c9a9fa85-4cdd-457e-b906-1a65e6e96f3d) |

## What was observed on a clean machine

Attempt 1:

- 10 min: `Rust toolchain not installed`
- `SoapySDR system library not found (feature soapy)`
- `ALSA system library not found (feature audio)`
- 3 min: `trybuild compile-fail stderr mismatched nightly 1.101.0 compiler output`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
