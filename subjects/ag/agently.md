# Agently

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/AgentEra/Agently, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/agently

## Pinned environment

- Project commit: `d58239501e7d4d2e50db26b6f9ebe20b86dc83a9`
- Test commit: `d58239501e7d4d2e50db26b6f9ebe20b86dc83a9`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 45.4 to 45.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 45.4 | 4 | 4 | [run](https://argusic.com/run/dd7e9def-fd89-402c-adee-d404edea1209) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Missing optional dependencies: python-dotenv, beautifulsoup4, fastapi, sqlmodel, aiosqlite, fastmcp`
- 2 min: `No python binary on PATH , only python3 available, but code adapters and providers hardcoded python as argv[0]`
- `9 characterization tests fail due to baseline snapshot drift (event paths and prompt content differ across package versions)`
- `test_gvisor_direct_docker_run_emits_one_fixed_runtime_argv fails , Docker daemon not available in container and monkeypatch does not cover inspect_availability()`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
