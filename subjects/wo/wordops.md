# WordOps

**Verdict: runs with mocks.** Argusic Score 84.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/WordOps/WordOps, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/wordops

## Pinned environment

- Project commit: `13a03e43df494b8f2e69378db732a3e8ced86a2c`
- Test commit: `13a03e43df494b8f2e69378db732a3e8ced86a2c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, no run possible
- Valid runs: 2; wall time 12.8 to 13.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 88.67 | 23 | 12.8 | 6 | 5 | [run](https://argusic.com/run/6fed0866-22d5-44d7-a764-898bea2392ee) |
| 2 | fail | 80 | 13.4 | 13.6 | 8 | 8 | [run](https://argusic.com/run/470a9ca1-84e9-4205-9ba0-b1fe09e5a4b6) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `ModuleNotFoundError: No module named 'imp' (nose incompatibility with Python 3.12)`
- 2 min: `ModuleNotFoundError: No module named 'pkg_resources'`
- 1 min: `PermissionError: copy2 ~/.gitconfig -> /root/.gitconfig`
- 5 min: `ModuleNotFoundError: No module named 'apt' (python3-apt system package not available)`
- 1 min: `PermissionError reading /proc/1/environ in grepcheck`
- `9 tests failed: require root/system packages (nginx, mysql) for integration testing`

Attempt 2:

- 6 min: `nose test runner incompatible with Python 3.12 (imp module removed, _TextTestResult renamed, collections.Callable removed)`
- 1.5 min: `pkg_resources not found with setuptools 84.x`
- 1 min: `variables.py tried to copy .gitconfig to /root/ (PermissionError as non-root)`
- 2 min: `aptget.py imports apt module not available (python3-apt not installed)`
- 1.5 min: `Plugin config files missing for cement framework`
- 2 min: `WOTestApp missing bootstrap/plugin_bootstrap Meta attributes`
- `non-root user cannot run wo CLI (designed to require root)`
- `37/80 tests errored due to infrastructure gaps (/proc/1/environ permission, missing /etc/nginx configs, 'pre_close' hook not registered in test WOTestApp)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
