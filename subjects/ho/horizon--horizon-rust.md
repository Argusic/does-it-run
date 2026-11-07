# horizon

**Verdict: runs.** Argusic Score 75 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/horizon-rust/horizon, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/run/a4c4ca18-1583-4a89-bc45-99f6bb9eff69

## Pinned environment

- Project commit: `56f968e11c7627536cb6a83420caddce7e3acb8f`
- Test commit: `56f968e11c7627536cb6a83420caddce7e3acb8f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 29.5 to 46.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 77 | 46.6 | 0 | 0 | [run](https://argusic.com/run/a4c4ca18-1583-4a89-bc45-99f6bb9eff69) |
| 2 | fail | 50 | 5 | 29.5 | 4 | 4 | [run](https://argusic.com/run/28192878-1e53-4f34-a4ea-ff2cf1859082) |

## What was observed on a clean machine

Attempt 2:

- `Missing libasound2-dev/libudev-dev (no root access; runtime libs exist, build works with --no-default-features)`
- `Missing libxcb-dev/libxkbcommon-dev (launcher fails to link)`
- `Game needs Minecraft 26.3 resources (horizon-prepare requires JDK 25 + real Minecraft installation)`
- `1 test fails on GLES (passes_chain_through_half_float_targets_with_options_and_depth)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
