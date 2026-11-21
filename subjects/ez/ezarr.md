# ezarr

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Luctia/ezarr, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/ezarr

## Pinned environment

- Project commit: `cc6a12a182d1805d7ef971d0737760e149f85110`
- Test commit: `cc6a12a182d1805d7ef971d0737760e149f85110`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 0.9 to 7.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 0.5 | 7.8 | 1 | 1 | [run](https://argusic.com/run/8ad989f9-4c5e-458c-a076-d0b7340bbd6a) |
| 2 | pass with mocks | 92 | 1 | 0.9 | 0 | 0 | [run](https://argusic.com/run/39ae582d-08ad-4b39-8901-0d1203d4a976) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `mylar3() method in container_configs.py missing TZ environment variable`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
