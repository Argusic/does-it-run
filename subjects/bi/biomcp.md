# biomcp

**Verdict: runs.** Argusic Score 94.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/genomoncology/biomcp, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/biomcp

## Pinned environment

- Project commit: `9e960ee32102f638e4a95e69e70b88264b496f07`
- Test commit: `9e960ee32102f638e4a95e69e70b88264b496f07`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 54.7 to 54.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 94.29 | 54 | 54.7 | 7 | 5 | [run](https://argusic.com/run/3ba3b749-8ecd-4232-842d-01f31c503ab6) |

## What was observed on a clean machine

Attempt 1:

- 15 min: `Rust toolchain (rustc, cargo) not pre-installed`
- 1 min: `uv package manager not pre-installed`
- 6 min: `cargo-nextest not pre-installed (required for test runner)`
- 5 min: `cargo-deny not pre-installed (required for lint)`
- 1 min: `mustmatch standalone binary not installed (required for spec contracts)`
- `bwrap user-namespace sandboxing unavailable (kernel restriction in container)`
- `Node.js v18.19.1 cannot execute ESM scripts in SDLC lifecycle tests (needs type:module)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
