# openworker

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/andrewyng/openworker, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/openworker

## Pinned environment

- Project commit: `5870585321e2cae0b2afbcd8903e14b63c959ac7`
- Test commit: `5870585321e2cae0b2afbcd8903e14b63c959ac7`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 6.1 to 28.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 28.1 | 0 | 0 | [run](https://argusic.com/run/d0a47001-8904-4256-9269-ace1eb02abcf) |
| 2 | pass | 100 | 4.5 | 6.1 | 0 | 0 | [run](https://argusic.com/run/dc8a8b32-42e0-4905-967f-7d55db0beeeb) |

## What was observed on a clean machine

No error was recorded during the valid runs.

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
