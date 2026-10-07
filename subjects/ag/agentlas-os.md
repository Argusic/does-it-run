# Agentlas-OS

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/agentlas-ai/Agentlas-OS, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/agentlas-os

## Pinned environment

- Project commit: `4ca8fd28d5ad9a92cbe33b39d05bcff8febe7448`
- Test commit: `4ca8fd28d5ad9a92cbe33b39d05bcff8febe7448`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 6.5 to 9.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 9.5 | 0 | 0 | [run](https://argusic.com/run/3593c9eb-22da-4856-ac64-407be46fb6e6) |
| 2 | pass | 100 | 6 | 6.5 | 2 | 2 | [run](https://argusic.com/run/ce1ddd9e-18e8-4d8d-b641-6156fd98af1f) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `install script failed to load host-adapter contract because agentlas_resolve_python_cmd requires system-wide jsonschema+referencing (checked via agentlas_python_candidate_ok); runtime home still deployed to ~/.agentlas/runtime/.generations`
- 0.5 min: `~/.local/bin/agentlas-one symlink not created by the installer on Linux`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
