# SemIf-OpenJev

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/TheoLeeCJ/SemIf-OpenJev, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/semif-openjev

## Pinned environment

- Project commit: `23cf1f39fc9534fe81437200959b6dfc7106e45a`
- Test commit: `23cf1f39fc9534fe81437200959b6dfc7106e45a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 3.8 to 9.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 6.5 | 9.2 | 0 | 0 | [run](https://argusic.com/run/6dc9b143-96f8-4be0-b1d8-9fa5e8d17dcb) |
| 2 | pass | 100 | 2.8 | 3.8 | 0 | 0 | [run](https://argusic.com/run/824b9271-e64a-431d-9481-830718b4970d) |

## What was observed on a clean machine

No error was recorded during the valid runs.

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
