# bustub

**Verdict: runs.** Argusic Score 83.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/cmu-db/bustub, licensed MIT, written in C++.

Evidence and recordings: https://argusic.com/subject/bustub

## Pinned environment

- Project commit: `c0a5431985287e258a6f25f53d822f0d0d2e63e8`
- Test commit: `c0a5431985287e258a6f25f53d822f0d0d2e63e8`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, no run possible
- Valid runs: 3; wall time 10 to 18.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 14.2 | 3 | 3 | [run](https://argusic.com/run/11a21750-a6ec-4667-8cd3-a900046f8395) |
| 2 | fail | 50 | 4 | 18.1 | 0 | 0 | [run](https://argusic.com/run/c388e043-cf7e-4c30-b4ca-3d0e0fa48ee4) |
| 3 | pass | 100 | 1 | 10 | 2 | 2 | [run](https://argusic.com/run/0446850b-eeea-4ca4-9f95-bec7cfb7de0e) |

## What was observed on a clean machine

Attempt 1:

- `clang-15 not available; only g++ 13 present`
- `libelf-dev and libdwarf-dev missing`
- `Interactive shell crashes on startup due to unimplemented BufferPoolManager`

Attempt 3:

- 1 min: `Missing libelf-dev and libdwarf-dev system packages`
- `Missing clang-15 compiler (using g++ 13 instead)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
