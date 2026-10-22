# radio-active

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/dpnkrpl/radio-active, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/radio-active

## Pinned environment

- Project commit: `cfc8d5d3479d780acb400554e83f2b9872ba0e53`
- Test commit: `cfc8d5d3479d780acb400554e83f2b9872ba0e53`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 2.9 to 2.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1.5 | 2.9 | 3 | 3 | [run](https://argusic.com/run/7f523bbd-6c00-4f71-bb79-ac67035dcbed) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `PEP 668 externally-managed-environment blocked system-wide pip install`
- 0.5 min: `pytest was not installed in venv`
- 1 min: `TypeError in handle_play_last_station when no last station saved`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
