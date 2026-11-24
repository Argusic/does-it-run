# harness-engineering

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/deusyu/harness-engineering, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/harness-engineering

## Pinned environment

- Project commit: `018f58d5f3189ce52777407e90b412130263a760`
- Test commit: `018f58d5f3189ce52777407e90b412130263a760`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 1.5 to 1.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1 | 1.5 | 0 | 0 | [run](https://argusic.com/run/b2ace8ad-73df-4fe8-ac0b-f79db34e41d8) |
| 2 | pass with mocks | 92 | 0.07 | 1.6 | 0 | 0 | [run](https://argusic.com/run/19bc2f8c-76fa-4a94-bd64-15272eadf2af) |

## What was observed on a clean machine

No error was recorded during the valid runs.

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
