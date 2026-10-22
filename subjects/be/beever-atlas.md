# beever-atlas

**Verdict: runs with mocks.** Argusic Score 56 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Beever-AI/beever-atlas, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/beever-atlas

## Pinned environment

- Project commit: `7d791af27ef4aa19644cb385c7ca24619bc4f848`
- Test commit: `7d791af27ef4aa19644cb385c7ca24619bc4f848`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 34.8 to 58.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 34.8 | 0 | 0 | [run](https://argusic.com/run/0211647a-cc5d-4299-bad9-6167c8fdeada) |
| 2 | pass with mocks | 92 | 1 | 58.1 | 2 | 2 | [run](https://argusic.com/run/1824ef2a-d254-4e8a-af3f-735e0c5bbabd) |

## What was observed on a clean machine

Attempt 2:

- `test_config: MONGODB_URI env override changes default assertion - .env has short timeout URI`
- `test_health: Redis not running on localhost:6379 causes health endpoint test to hang`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
