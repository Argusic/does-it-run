# excel-mcp-server

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/haris-musa/excel-mcp-server, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/excel-mcp-server

## Pinned environment

- Project commit: `f51340ecd5778952405044b203d3a2d4c8a46833`
- Test commit: `f51340ecd5778952405044b203d3a2d4c8a46833`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, no run possible
- Valid runs: 2; wall time 3.8 to 4.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.35 | 3.8 | 2 | 2 | [run](https://argusic.com/run/5efba375-8932-4ab3-8c8f-af10729eb02f) |
| 2 | fail | 20 | n/a | 4.6 | 0 | 0 | [run](https://argusic.com/run/e195d379-4db1-493a-bf13-60ec68b01bfd) |

## What was observed on a clean machine

Attempt 1:

- 0.05 min: `pip install failed: externally-managed-environment`
- `Server print to closed stdout in stdio mode when stdin closes prematurely`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
