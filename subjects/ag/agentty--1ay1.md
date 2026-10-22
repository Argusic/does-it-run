# agentty

**Verdict: could not verify.** Argusic Score 50 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/1ay1/agentty, licensed MIT, written in C++.

Evidence and recordings: https://argusic.com/run/5332b82e-41be-4722-8120-a68742838e69

## Pinned environment

- Project commit: `23560a0487bd35aa2863da5114b88889656c94a6`
- Test commit: `23560a0487bd35aa2863da5114b88889656c94a6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 2; wall time 15.7 to 29.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 15.7 | 0 | 0 | [run](https://argusic.com/run/5332b82e-41be-4722-8120-a68742838e69) |
| 2 | fail | 80 | 33 | 29.7 | 4 | 4 | [run](https://argusic.com/run/c45c9ee9-48ce-43ca-bf0b-e1c32b6da0f0) |

## What was observed on a clean machine

Attempt 2:

- 33 min: `Source build fails: jaal dependency needs C++26 structured binding packs (P1061) which require Clang 22+ or GCC 16+. Available compiler is Clang 19.1.7 (via LLVM prebuilt).`
- 10 min: `libnghttp2-dev not installed in container (only libnghttp2-14 shared lib present). Headers missing for find_path/find_library.`
- 5 min: `CMake 3.28.3 was too old for jaal submodule (req 3.29+).`
- 5 min: `maya CMakeLists.txt hard-failed on C++26 detection with GCC 13 (no -std=c++2c).`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
