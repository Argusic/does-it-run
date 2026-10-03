# adk-python

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/google/adk-python, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/adk-python

## Pinned environment

- Project commit: `9625b06c9a1be6b9ecd85225657690ae5c0e9d3e`
- Test commit: `9625b06c9a1be6b9ecd85225657690ae5c0e9d3e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 13.6 to 58.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 58.9 | 0 | 0 | [run](https://argusic.com/run/0849274b-6637-494a-845e-4257cf5d9f8d) |
| 2 | pass | 100 | 0.5 | 13.6 | 1 | 1 | [run](https://argusic.com/run/a33ce9d1-4407-4d89-a357-1749004308af) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `test_entry_point_loads_only_allowlisted_packages failed: sitecustomize (system apport hook) loaded at interpreter startup not in allowlist`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
