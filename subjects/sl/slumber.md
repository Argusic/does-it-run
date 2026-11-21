# slumber

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/LucasPickering/slumber, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/slumber

## Pinned environment

- Project commit: `0697b7adcc415ccd3a22e12a015f9eab7a4bacd7`
- Test commit: `0697b7adcc415ccd3a22e12a015f9eab7a4bacd7`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 7.8 to 16.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 16.5 | 2 | 2 | [run](https://argusic.com/run/3b250dc2-a2bc-4b70-9b01-5cf5f8f66af0) |
| 2 | pass | 100 | 8 | 7.8 | 2 | 2 | [run](https://argusic.com/run/5e5d4714-1d4a-4c50-88b3-4ceb60db8a23) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `Rust toolchain missing in container (cargo/rustc not found)`
- 7 min: `Workspace test suite failed to link slumber_python: rust-lld: unable to find library -lpython3.12`

Attempt 2:

- 1 min: `slumber_python crate fails to compile: missing -lpython3.12 shared library`
- 0.5 min: `TUI panics with 'reader source not set' in non-interactive/headless terminal`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
