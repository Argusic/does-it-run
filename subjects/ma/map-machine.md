# map-machine

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/enzet/map-machine, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/map-machine

## Pinned environment

- Project commit: `eab10c1ec9bcd0a78fa6db75d02e6219fcea562c`
- Test commit: `eab10c1ec9bcd0a78fa6db75d02e6219fcea562c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 6.8 to 6.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8 | 6.8 | 4 | 4 | [run](https://argusic.com/run/ba8ad664-325c-4c57-812f-265f85186405) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `PEP 668 externally-managed-environment blocked pip install`
- 0.5 min: `pytest not installed in venv`
- 1 min: `10 command-line tests failed: 'map-machine' not in subprocess PATH`
- 5 min: `Rendering crash: $industrial_opacity variable not resolved for way opacity (power_opacity -> $industrial_opacity not recursively resolved)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
