# wreq

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/0x676e67/wreq, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/wreq

## Pinned environment

- Project commit: `2ff34c3e512e28e968f871339081d1e47f64750a`
- Test commit: `2ff34c3e512e28e968f871339081d1e47f64750a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 34.7 to 49.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 49.7 | 0 | 0 | [run](https://argusic.com/run/3c673163-f449-4921-b20d-0420f8d333b1) |
| 2 | pass | 100 | 10 | 34.7 | 3 | 3 | [run](https://argusic.com/run/310967ba-7b4c-467e-9f97-1fb91e51d781) |

## What was observed on a clean machine

Attempt 2:

- 0.2 min: `Rust toolchain not found in container`
- 3 min: `libclang.so not found - bindgen failed to generate BoringSSL FFI bindings`
- 2 min: `stddef.h not found by clang when parsing BoringSSL headers (Ubuntu 24.04 libc6-dev no longer ships /usr/include/stddef.h)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
