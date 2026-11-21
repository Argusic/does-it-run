# OpenOutreach

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/eracle/OpenOutreach, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/openoutreach

## Pinned environment

- Project commit: `85c9367ed3291d984013921a85fa659426b96849`
- Test commit: `85c9367ed3291d984013921a85fa659426b96849`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 1.8 to 2.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 6.5 | 1.8 | 0 | 0 | [run](https://argusic.com/run/10d07c2a-ab15-4e72-8ad5-4ccd46ce81aa) |
| 2 | pass | 100 | 22 | 2.1 | 2 | 2 | [run](https://argusic.com/run/937abf27-969d-4eb3-9240-dadb75c25c69) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `pip3 install uv failed: PEP 668 external-managed-environment restriction`
- 1 min: `make setup failed because uv not in PATH in sh subshell`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
