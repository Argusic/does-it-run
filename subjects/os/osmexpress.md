# OSMExpress

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/bdon/OSMExpress, licensed BSD-2-Clause, written in C++.

Evidence and recordings: https://argusic.com/subject/osmexpress

## Pinned environment

- Project commit: `045a515132e91a3679ce3df27329937c9b8b221a`
- Test commit: `045a515132e91a3679ce3df27329937c9b8b221a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 13.7 to 13.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 10 | 13.7 | 3 | 3 | [run](https://argusic.com/run/9249163d-289f-41f4-8b35-ce26fd64643d) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `CMakeLists.txt hardcoded clang compilers not present`
- 3 min: `System missing libbz2-dev, zlib1g-dev, libexpat1-dev headers and libs`
- 1 min: `CMakeLists.txt had three consecutive set(CMAKE_CXX_FLAGS ...) lines that each overwrote previous value`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
