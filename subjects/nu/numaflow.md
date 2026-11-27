# numaflow

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/numaproj/numaflow, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/numaflow

## Pinned environment

- Project commit: `4ee902439445edea365bf88940df2abab11b2f57`
- Test commit: `4ee902439445edea365bf88940df2abab11b2f57`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 39.7 to 39.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 39 | 39.7 | 5 | 5 | [run](https://argusic.com/run/34632f36-2b20-4d78-9db2-8590caeaddab) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Go compiler not found in container`
- 2 min: `Rust toolchain not found in container`
- 3 min: `libclang missing for Rust bindgen crate`
- 1 min: `protoc missing for Rust pulsar crate`
- 1 min: `stddef.h not found by clang-based bindgen`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
