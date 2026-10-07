# ladybird

**Verdict: runs.** Argusic Score 93.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/LadybirdBrowser/ladybird, licensed BSD-2-Clause, written in C++.

Evidence and recordings: https://argusic.com/subject/ladybird

## Pinned environment

- Project commit: `a71cffae5ad9d29729bb3364a49a637895286e1f`
- Test commit: `a71cffae5ad9d29729bb3364a49a637895286e1f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 7.8 to 7.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 93.33 | 6 | 7.8 | 3 | 2 | [run](https://argusic.com/run/fe13f4ce-4baa-40d3-b6cd-d784bc110364) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Rust toolchain not installed`
- `Python meta tests required LADYBIRD_SOURCE_DIR env var`
- 2 min: `Full C++/CMake build requires CMake 3.30+, Qt 6.10+, libedit, ninja, and other dependencies not available without root`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
