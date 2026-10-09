# MCPJungle

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/mcpjungle/MCPJungle, licensed MPL-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/mcpjungle

## Pinned environment

- Project commit: `12648be5edc70391dc3f9c4aecfd37b83b3e30be`
- Test commit: `12648be5edc70391dc3f9c4aecfd37b83b3e30be`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 14.1 to 14.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 18 | 14.1 | 2 | 2 | [run](https://argusic.com/run/4d798ed9-e49f-4e4c-a823-70528fe56553) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Go compiler not installed in container`
- 2 min: `Dashboard UI bundle missing from internal/dashboardui/dist, blocking Go build`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
