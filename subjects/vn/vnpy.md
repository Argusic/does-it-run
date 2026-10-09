# vnpy

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/vnpy/vnpy, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/vnpy

## Pinned environment

- Project commit: `c6e231caf32b7fc97e6459817fff66458cf7e7c4`
- Test commit: `c6e231caf32b7fc97e6459817fff66458cf7e7c4`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 7 to 7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 4.5 | 7 | 4 | 4 | [run](https://argusic.com/run/dbae8635-8909-4fd4-ba59-fe1c97975c37) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `Missing dependency: statsmodels (imported by vnpy.alpha.dataset.factor_performance)`
- 0.2 min: `Missing dependency: vnpy-sqlite (imported by test_data_services.py)`
- 0.2 min: `Missing dependency: pytest (needed for test runner)`
- 0.3 min: `xcb platform plugin fails: missing libxcb-cursor0 system package (not installable without root)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
