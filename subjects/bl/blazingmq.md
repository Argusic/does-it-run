# blazingmq

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/bloomberg/blazingmq, licensed Apache-2.0, written in C++.

Evidence and recordings: https://argusic.com/subject/blazingmq

## Pinned environment

- Project commit: `9eb4b19ee056d1d0ae7c6a473fbb33d9e8f32fa9`
- Test commit: `9eb4b19ee056d1d0ae7c6a473fbb33d9e8f32fa9`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 75.1 to 87 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | n/a | 87 | 0 | 0 | [run](https://argusic.com/run/22747a8e-1e65-4cef-940f-b410639de326) |
| 2 | pass | 100 | 75 | 75.1 | 4 | 4 | [run](https://argusic.com/run/0b08cfc1-a710-4071-9762-2450282eb011) |

## What was observed on a clean machine

Attempt 2:

- 5 min: `Missing build tools packages (flex, bison, m4, ninja, benchmark, zlib-dev) - no root access`
- 2 min: `Bison could not find m4 binary and data files`
- 3 min: `Missing pkg-config .pc files for zlib, benchmark, gtest`
- 1 min: `CMake FLEX_INCLUDE_DIR not found`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
