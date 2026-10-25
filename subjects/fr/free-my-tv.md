# free-my-tv

**Verdict: runs with mocks.** Argusic Score 86 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/simbasjungles/free-my-tv, licensed MIT, written in Java.

Evidence and recordings: https://argusic.com/subject/free-my-tv

## Pinned environment

- Project commit: `aa34335d25fa2224053d1bb16851e4522a6bbeb0`
- Test commit: `aa34335d25fa2224053d1bb16851e4522a6bbeb0`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 2 to 3.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 5 | 2 | 0 | 0 | [run](https://argusic.com/run/4bb70411-7a05-4c68-a224-c2c4cb93cba2) |
| 2 | pass with mocks | 92 | 5 | 3.2 | 0 | 0 | [run](https://argusic.com/run/9c1d638f-2009-4564-aec3-edea4c713896) |

## What was observed on a clean machine

No error was recorded during the valid runs.

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
