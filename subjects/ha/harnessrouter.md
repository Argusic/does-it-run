# harnessrouter

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/HarnessRouter/harnessrouter, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/harnessrouter

## Pinned environment

- Project commit: `fc8da524f408758e5420a1a415fe5e45e494aa33`
- Test commit: `fc8da524f408758e5420a1a415fe5e45e494aa33`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 5.5 to 17.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 15 | 17.4 | 1 | 1 | [run](https://argusic.com/run/eab0e9df-d8ef-4ee3-81e2-ffb128b022cd) |
| 2 | pass | 100 | 1.2 | 5.5 | 0 | 0 | [run](https://argusic.com/run/ff2bce52-cfbe-4d38-8e2c-c6a21ccdd387) |

## What was observed on a clean machine

Attempt 1:

- 10 min: `Next.js build OOM-killed during static page generation with default Node memory (8 GB container limit, but Next.js static generation exceeds available heap)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
