# unqlite-python

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/coleifer/unqlite-python, licensed MIT, written in C.

Evidence and recordings: https://argusic.com/subject/unqlite-python

## Pinned environment

- Project commit: `b42c6aa4e53af15a8d8851017016f5883a20a4e4`
- Test commit: `b42c6aa4e53af15a8d8851017016f5883a20a4e4`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 2.6 to 7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.25 | 2.6 | 1 | 1 | [run](https://argusic.com/run/e30bb5f1-f4ba-45af-be3b-6b9515cbcc19) |
| 2 | pass | 100 | 2.5 | 7 | 3 | 3 | [run](https://argusic.com/run/fce5d3d9-adef-4a3f-bc11-85636b1aaeb9) |

## What was observed on a clean machine

Attempt 1:

- 0.1 min: `Building from source failed: /usr/include/python3.12/Python.h missing (python3-dev not installed)`

Attempt 2:

- 0.2 min: `pip install fails with externally-managed-environment (PEP 668)`
- 0.8 min: `build fails: Python.h: No such file or directory (missing python3-dev headers, no root)`
- 0.3 min: `build fails: nested pyconfig.h include for x86_64-linux-gnu/python3.12/pyconfig.h not found`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
