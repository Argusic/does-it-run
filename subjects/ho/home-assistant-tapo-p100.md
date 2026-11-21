# home-assistant-tapo-p100

**Verdict: runs with mocks.** Argusic Score 56 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/petretiandrea/home-assistant-tapo-p100, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/home-assistant-tapo-p100

## Pinned environment

- Project commit: `a0e1a30736579ea5e1f7f7b8c6aedc0bb70b2cdc`
- Test commit: `a0e1a30736579ea5e1f7f7b8c6aedc0bb70b2cdc`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, no run possible
- Valid runs: 2; wall time 0.4 to 32.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 30 | 32.1 | 7 | 7 | [run](https://argusic.com/run/77995fb7-7674-4b49-88ad-520cf96f8a32) |
| 2 | fail | 20 | n/a | 0.4 | 0 | 0 | [run](https://argusic.com/run/0a5adcf8-fc70-4aa0-8e79-99e7b466e316) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `uv not installed in container`
- 6 min: `project requires Python >=3.14.2, system has 3.12.3`
- 6 min: `libffi-dev missing (ffi.h not found) - needed to build cffi`
- `pydantic-core build failed: PyO3 0.26.0 max supported version is 3.14 (uv installed Python 3.15)`
- `pillow build failed: missing zlib headers for source build (Python 3.15 had no wheel)`
- 1 min: `config check: Integration 'tapo' not found`
- 3 min: `HA crash/hang on subsequent launches due to stale .storage and .ha_run.lock files`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
