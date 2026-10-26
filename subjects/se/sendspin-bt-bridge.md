# sendspin-bt-bridge

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/trudenboy/sendspin-bt-bridge, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/sendspin-bt-bridge

## Pinned environment

- Project commit: `38762b5ebbf0a295af8f5da6c2ccbbb07992b82d`
- Test commit: `38762b5ebbf0a295af8f5da6c2ccbbb07992b82d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 13.6 to 13.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 35 | 13.6 | 2 | 2 | [run](https://argusic.com/run/2dbf87c3-2309-474c-b755-75482199c346) |

## What was observed on a clean machine

Attempt 1:

- 12 min: `pycairo build fails: missing libcairo2-dev (no root) and no python3.pc for meson; PyGObject needs gi from system python3-gi apt package`
- 5 min: `ModuleNotFoundError: No module named gi at test collection (gst_support.py imports gi at module level)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
