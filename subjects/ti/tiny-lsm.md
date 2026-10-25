# tiny-lsm

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Vanilla-Beauty/tiny-lsm, licensed MIT, written in C++.

Evidence and recordings: https://argusic.com/subject/tiny-lsm

## Pinned environment

- Project commit: `838b53b6e989c1a5efa36e2a136b0e3a775b517a`
- Test commit: `838b53b6e989c1a5efa36e2a136b0e3a775b517a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 15.2 to 15.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 15.2 | 4 | 4 | [run](https://argusic.com/run/7f3af560-5e3d-46b3-91b4-81eb50661849) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `gmock package not available in xmake-repo`
- 2 min: `pybind11 requires Python dev headers not installed`
- 1 min: `unzip binary not available in container`
- 1 min: `xmake local-repo 'build' directory didn't exist`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
