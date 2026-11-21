# agy-staff

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/keli-wen/agy-staff, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/agy-staff

## Pinned environment

- Project commit: `8a69f0a8a02f3d159e0e6c3ed52ce054ce814592`
- Test commit: `8a69f0a8a02f3d159e0e6c3ed52ce054ce814592`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 2.6 to 46.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 0.5 | 2.6 | 0 | 0 | [run](https://argusic.com/run/348fd344-7d46-454e-8e92-c0d41d940373) |
| 2 | pass with mocks | 92 | 0 | 46.2 | 1 | 1 | [run](https://argusic.com/run/7ddc7d21-3383-4bd0-aa9d-efb35e9ed792) |

## What was observed on a clean machine

Attempt 2:

- `Flaky timing race in terminal-observation.test.mjs: observe during a pending wait never duplicates its large final report test (competing background wait vs observe read may finish before observe is called)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
