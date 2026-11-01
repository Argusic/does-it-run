# dsh-antibrow

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/antibrow/dsh-antibrow, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/dsh-antibrow

## Pinned environment

- Project commit: `d032210ba3f5747686fb151fc79d2bc9a89c2ea4`
- Test commit: `d032210ba3f5747686fb151fc79d2bc9a89c2ea4`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 10.6 to 10.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 0.5 | 10.6 | 3 | 3 | [run](https://argusic.com/run/cc800bed-6c78-4931-b229-8afc185907cc) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Promise.withResolvers is not a function in Node 18.19.1, crashing dsh-mcp-client plugin at connectGeneration()`
- 2 min: `Mock MCP server had wrong SDK import paths (dist/esm/server/mcp.js resolved to double dist/esm/ path)`
- 10 min: `No ANTI_DETECT_BROWSER_KEY available and Playwright requires Node 20+`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
