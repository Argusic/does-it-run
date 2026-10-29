# agent-browser-mcp

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/335234131/agent-browser-mcp, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/agent-browser-mcp

## Pinned environment

- Project commit: `04cc1f1e94bb9c9692aa2abb702d5adb9917923b`
- Test commit: `04cc1f1e94bb9c9692aa2abb702d5adb9917923b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 27.8 to 27.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 28 | 27.8 | 3 | 3 | [run](https://argusic.com/run/a45f43d8-6b75-4e8f-af25-471e06de2c81) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `pip install -e . failed: externally-managed-environment (PEP 668)`
- 5 min: `mcp 2.3.0 installed; repo imports mcp.server.fastmcp (v1 API) -> ModuleNotFoundError on every CLI command`
- 6 min: `doctor always reports http_port_open:false for port 18766 while the HTTP bridge actually binds (raw TCP check races previous run's port state)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
