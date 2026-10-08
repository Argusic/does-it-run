# rosenpass

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/rosenpass/rosenpass, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/rosenpass

## Pinned environment

- Project commit: `89a8805b4da8ad1d4bab313e6929bc1fb9016977`
- Test commit: `89a8805b4da8ad1d4bab313e6929bc1fb9016977`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 9.9 to 9.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 25 | 9.9 | 3 | 3 | [run](https://argusic.com/run/cb03ab36-c3eb-46d7-a689-cc64ce7d70a0) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `rustc/cargo not found in container`
- 8 min: `libclang not found for bindgen in oqs-sys build`
- 2 min: `clang resource headers missing from libclang-20-dev package`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
