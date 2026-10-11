# onetun

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/aramperes/onetun, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/onetun

## Pinned environment

- Project commit: `3ca5ae2181f17a2ed12009c578b8f25ab82ce6f8`
- Test commit: `3ca5ae2181f17a2ed12009c578b8f25ab82ce6f8`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 6.7 to 6.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 6 | 6.7 | 1 | 1 | [run](https://argusic.com/run/cc9cb174-8f01-4e67-a105-e693e89c6a0e) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `cargo/rustc (Rust toolchain) not installed in container; README requires Rust >=1.80.0`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
