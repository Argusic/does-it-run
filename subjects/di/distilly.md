# distilly

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/titanwings/distilly, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/distilly

## Pinned environment

- Project commit: `b830d3dcbde006370f141155795b89021e3a947b`
- Test commit: `b830d3dcbde006370f141155795b89021e3a947b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 2.1 to 3.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 0.7 | 3.6 | 0 | 0 | [run](https://argusic.com/run/6dc1878b-a6ce-4782-877b-0f725c2dfd82) |
| 2 | pass | 100 | 27 | 2.1 | 0 | 0 | [run](https://argusic.com/run/4e193d03-2228-45ba-814a-1715c3f7ed5c) |

## What was observed on a clean machine

No error was recorded during the valid runs.

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
