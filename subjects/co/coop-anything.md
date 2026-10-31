# coop-anything

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/cranebeaker/coop-anything, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/coop-anything

## Pinned environment

- Project commit: `b494a3f3dfd1cee76fcd869ebe217760be2d0e18`
- Test commit: `b494a3f3dfd1cee76fcd869ebe217760be2d0e18`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 31.4 to 31.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 14 | 31.4 | 3 | 3 | [run](https://argusic.com/run/73198510-99ed-459e-b76f-07f83cd82828) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `PEP 668 blocked system pip install of PyYAML for the MCP server (README/playbook/mcp.md requires it)`
- 10 min: `tools/buildlock/run_tests.py mutation twin check_msvc_environment[vcvars_ignored] could never be caught on non-Windows: check_msvc_environment bails out early, so the vcvars_env patch was unobservable`
- 2 min: `tools/mcp/coop_mcp.py detect_engine silently returned same_engine_projects: [] when PyYAML was missing, so MCP clients got wrong engine-family data`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
