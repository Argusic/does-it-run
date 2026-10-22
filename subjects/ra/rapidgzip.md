# rapidgzip

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/mxmlnkn/rapidgzip, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/rapidgzip

## Pinned environment

- Project commit: `d2350e9c9ba54398cd64e45bfc8c631beec017f0`
- Test commit: `d2350e9c9ba54398cd64e45bfc8c631beec017f0`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 7.9 to 7.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 7.9 | 5 | 5 | [run](https://argusic.com/run/60e02300-c589-4648-baf3-fe7f0fa63d50) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `PEP 668 blocked system pip install`
- 2 min: `test deps pytest/numpy/indexed_bzip2 missing`
- 1 min: `pytest testGIL.py failed 2 tests without -X dev`
- 1 min: `unclosed RapidgzipFile aborts at interpreter exit with finalization message`
- 3 min: `source build failed: Python.h not found (no python3-dev, no root)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
