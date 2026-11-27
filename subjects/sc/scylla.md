# scylla

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/MikeChongCan/scylla, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/scylla

## Pinned environment

- Project commit: `1c95cf795eafeeed3a2acf064e1786ff304fdbc4`
- Test commit: `1c95cf795eafeeed3a2acf064e1786ff304fdbc4`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 9.6 to 9.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 2.5 | 9.6 | 5 | 5 | [run](https://argusic.com/run/3ad479c2-2aff-436a-84ea-394c942c0072) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `Externally-managed Python environment blocks pip install`
- 0.2 min: `tests/cli_test.py: RuntimeError 'Directory /work/repo/scylla/assets does not exist' - starlette StaticFiles mount at import time`
- 0.2 min: `tests/validator_test.py::test_latency: OSError [Errno 113] No route to host uncaught in tcpping.py`
- 0.2 min: `tests/worker_test.py: Chromium 'chrome' not found at /opt/google/chrome/chrome`
- 0.1 min: `scheduler.py::stop(): AttributeError on worker_process.terminate() when scheduler not started`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
