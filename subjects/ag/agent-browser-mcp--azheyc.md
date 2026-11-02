# agent-browser-mcp

**Verdict: runs with mocks.** Argusic Score 86 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Azheyc/agent-browser-mcp, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/run/a172ad66-1c8a-4f8e-b951-4be3aea6348f

## Pinned environment

- Project commit: `04cc1f1e94bb9c9692aa2abb702d5adb9917923b`
- Test commit: `04cc1f1e94bb9c9692aa2abb702d5adb9917923b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 4.5 to 5.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 4 | 4.5 | 2 | 2 | [run](https://argusic.com/run/a172ad66-1c8a-4f8e-b951-4be3aea6348f) |
| 2 | pass with mocks | 92 | 2 | 5.6 | 2 | 2 | [run](https://argusic.com/run/a5980959-70b7-4703-8b4c-3f2be9d37317) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `mcp 2.x was installed (FastMCP renamed to MCPServer), breaking import`
- `mouseinfo requires tkinter (not installed, can't install without root), blocking pyautogui pointer functions`

Attempt 2:

- 1 min: `mcp v2 renamed FastMCP to MCPServer; import failed`
- 1 min: `mouseinfo calls sys.exit() when tkinter is missing on Linux`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
