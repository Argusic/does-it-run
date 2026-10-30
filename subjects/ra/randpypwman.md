# RandPyPwMan

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/HaydenHildreth/RandPyPwMan, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/randpypwman

## Pinned environment

- Project commit: `4bb971918130ecd3cf36cbbcfc0ee59614efbc7b`
- Test commit: `4bb971918130ecd3cf36cbbcfc0ee59614efbc7b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 5.8 to 6.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 6.1 | 0 | 0 | [run](https://argusic.com/run/7a7609bd-a2c8-429a-a6fa-4c9761a2453d) |
| 2 | pass | 100 | 8 | 5.8 | 3 | 3 | [run](https://argusic.com/run/ea76cd6a-49d1-4320-b69c-749cd89b499e) |

## What was observed on a clean machine

Attempt 2:

- 5 min: `python3-tk not installed (no tkinter module)`
- 1 min: `pip install tk (PyPI stub) did not actually provide tkinter`
- `source command not available in /bin/sh`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
