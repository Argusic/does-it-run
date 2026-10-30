# hermes-life-os

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Lethe044/hermes-life-os, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/hermes-life-os

## Pinned environment

- Project commit: `f754672e331d307bcb8575d60345d75681230eba`
- Test commit: `f754672e331d307bcb8575d60345d75681230eba`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 2 to 2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 15 | 2 | 3 | 3 | [run](https://argusic.com/run/801e73b8-e500-46bb-a704-4d4c009eb633) |

## What was observed on a clean machine

Attempt 1:

- `python command not found (only python3)`
- 1 min: `pip install failed: externally-managed-environment`
- 1 min: `5 test_dashboard.py tests failed: ImportError for matplotlib`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
