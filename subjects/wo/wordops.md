# WordOps

**Verdict: runs with mocks.** Argusic Score 88.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/WordOps/WordOps, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/wordops

## Pinned environment

- Project commit: `13a03e43df494b8f2e69378db732a3e8ced86a2c`
- Test commit: `13a03e43df494b8f2e69378db732a3e8ced86a2c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 12.8 to 12.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 88.67 | 23 | 12.8 | 6 | 5 | [run](https://argusic.com/run/6fed0866-22d5-44d7-a764-898bea2392ee) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `ModuleNotFoundError: No module named 'imp' (nose incompatibility with Python 3.12)`
- 2 min: `ModuleNotFoundError: No module named 'pkg_resources'`
- 1 min: `PermissionError: copy2 ~/.gitconfig -> /root/.gitconfig`
- 5 min: `ModuleNotFoundError: No module named 'apt' (python3-apt system package not available)`
- 1 min: `PermissionError reading /proc/1/environ in grepcheck`
- `9 tests failed: require root/system packages (nginx, mysql) for integration testing`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
