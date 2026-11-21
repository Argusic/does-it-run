# cdp-bridge-mcp

**Verdict: runs with mocks.** Argusic Score 86 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Unagi-cq/cdp-bridge-mcp, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/cdp-bridge-mcp

## Pinned environment

- Project commit: `cc33c4161f2968fb5c24a72fce9efd158e737856`
- Test commit: `cc33c4161f2968fb5c24a72fce9efd158e737856`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 2.7 to 5.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 3 | 2.7 | 0 | 0 | [run](https://argusic.com/run/96358dbf-4cee-4107-8b75-f838db99a230) |
| 2 | pass with mocks | 92 | 0.5 | 5.1 | 0 | 0 | [run](https://argusic.com/run/50a41e32-50e5-48a2-b51e-7c014c628307) |

## What was observed on a clean machine

No error was recorded during the valid runs.

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
