# KiCAD-MCP-Server

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/mixelpixx/KiCAD-MCP-Server, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/kicad-mcp-server

## Pinned environment

- Project commit: `670d2a9c48e1588f2e07edaf656b5e301fc55a50`
- Test commit: `670d2a9c48e1588f2e07edaf656b5e301fc55a50`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 5.4 to 5.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 5 | 5.4 | 1 | 1 | [run](https://argusic.com/run/1136b8b4-ba3e-437e-b2e8-093ce723a58a) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `System Python refused pip install (externally-managed-environment)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
