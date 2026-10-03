# kev

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/jaredpalmer/kev, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/kev

## Pinned environment

- Project commit: `3e1cd3bb588a388a06827443380befece23e68c7`
- Test commit: `3e1cd3bb588a388a06827443380befece23e68c7`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 62.6 to 62.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 1.5 | 62.6 | 4 | 4 | [run](https://argusic.com/run/42c80365-1525-462d-b423-cec8131305fa) |

## What was observed on a clean machine

Attempt 1:

- `test_api.py: all 10 tests fail , require running kev.serve`
- 2 min: `test_model.py: OOM-killed (8GB cgroup limit) or skipped`
- 3 min: `test_unit.py: 8 full_weight/interpolation tests hang on CPU (train tiny models, exceed 8GB limit)`
- 5 min: `Smoke training OOMs on CPU under 8GB cgroup limit`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
