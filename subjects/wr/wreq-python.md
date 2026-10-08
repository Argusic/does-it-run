# wreq-python

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/0x676e67/wreq-python, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/wreq-python

## Pinned environment

- Project commit: `24be2b62085472366d2dcac9f34a376921359a41`
- Test commit: `24be2b62085472366d2dcac9f34a376921359a41`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 14.5 to 14.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 9.5 | 14.5 | 3 | 3 | [run](https://argusic.com/run/d8a7a2b9-97e4-4826-8a64-ab100855e2a7) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `Rust toolchain (rustc/cargo) not found in container`
- 7 min: `bindgen-0.72.1 could not find libclang (libclang.so)`
- 2 min: `Tests fail with ConnectionError to localhost:8080 (no httpbin service)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
