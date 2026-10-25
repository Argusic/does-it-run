# searcharray

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/softwaredoug/searcharray, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/searcharray

## Pinned environment

- Project commit: `5ead0c721128d506264be33d9445e9a8508c5f98`
- Test commit: `5ead0c721128d506264be33d9445e9a8508c5f98`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 35 to 35 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 35 | 2 | 2 | [run](https://argusic.com/run/c4c13d20-0a24-453e-ba1d-306ea9c9caa8) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `sortednp fails to build from source - needs Python.h (python3-dev)`
- 5 min: `libpython3.12-dev not installed - Cython extensions cannot find Python.h or pyconfig.h`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
