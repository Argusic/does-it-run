# kk-mix

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/jaikydota/kk-mix, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/kk-mix

## Pinned environment

- Project commit: `01077fabc17e6ac69a1bd0b156cdf34224aba953`
- Test commit: `01077fabc17e6ac69a1bd0b156cdf34224aba953`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 5.6 to 5.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 5.6 | 2 | 2 | [run](https://argusic.com/run/def20385-06e9-4e8e-85cf-f206a3b61789) |

## What was observed on a clean machine

Attempt 1:

- `libxcb-cursor0 system library not found , Qt xcb platform plugin cannot load (xcb-cursor0 missing)`
- `Cython compile of _license_core.pyx fails , Python.h not found (python3-dev headers missing, no root)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
