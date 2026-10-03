# tsurugidb

**Verdict: could not verify.** Argusic Score 20 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/project-tsurugi/tsurugidb, licensed Apache-2.0, written in Shell.

Evidence and recordings: https://argusic.com/subject/tsurugidb

## Pinned environment

- Project commit: `555e8160047c44fe6215566369dd2e669bbc1694`
- Test commit: `555e8160047c44fe6215566369dd2e669bbc1694`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 2; wall time 7.6 to 30.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 30.5 | 0 | 0 | [run](https://argusic.com/run/ebcb4886-28e8-46ee-a68b-316e36ef6858) |
| 2 | fail | 20 | 11 | 7.6 | 1 | 1 | [run](https://argusic.com/run/c50dfc6b-f02f-486b-bb32-153943698ed3) |

## What was observed on a clean machine

Attempt 2:

- `The environment (Ubuntu 24.04, x86_64 container as user 'runner' with no root/sudo and no docker) lacks all 27+ system packages required to build Tsurugi from source: Boost (libboost-container-dev, libboost-filesystem-dev, libboost-regex-de`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
