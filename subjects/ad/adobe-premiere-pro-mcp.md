# Adobe_Premiere_Pro_MCP

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/hetpatel-11/Adobe_Premiere_Pro_MCP, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/adobe-premiere-pro-mcp

## Pinned environment

- Project commit: `ee31c3def7c3ca1c68662ea7737a9f8e5a2b634f`
- Test commit: `ee31c3def7c3ca1c68662ea7737a9f8e5a2b634f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 13.9 to 13.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 5 | 13.9 | 1 | 1 | [run](https://argusic.com/run/1fb4ddb0-64ee-4d56-b8a9-0f5f466708cb) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `CLI --version flag uses Node 20-only import assertion (import ... with { type: 'json' })`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
