# autoclip

**Verdict: runs.** Argusic Score 90.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/zhouxiaoka/autoclip, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/autoclip

## Pinned environment

- Project commit: `17100c05252b9a947ea1a857f8d0ea4f3af2317b`
- Test commit: `17100c05252b9a947ea1a857f8d0ea4f3af2317b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 3; wall time 3.6 to 10.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 4 | 8.6 | 0 | 0 | [run](https://argusic.com/run/260e7e15-9703-491d-bf1d-594d0b76a38f) |
| 2 | pass | 100 | 2 | 10.5 | 0 | 0 | [run](https://argusic.com/run/3f1ca862-424d-4bd7-89c0-474e8bcebd6a) |
| 3 | pass | 80 | 5 | 3.6 | 2 | 0 | [run](https://argusic.com/run/7d1d2dd4-fc99-441e-afe7-8d95576fcaa1) |

## What was observed on a clean machine

Attempt 3:

- 2 min: `Redis server not available (cannot install system packages without root)`
- `No DashScope API key configured (API_DASHSCOPE_API_KEY is empty)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
