# mcp-server-chart

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/antvis/mcp-server-chart, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/mcp-server-chart

## Pinned environment

- Project commit: `e2a8fb7c185e17c75c067817ff1a2acfddf49aa1`
- Test commit: `e2a8fb7c185e17c75c067817ff1a2acfddf49aa1`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 37.8 to 37.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 37 | 37.8 | 3 | 3 | [run](https://argusic.com/run/3c481f48-dc51-45c8-a930-efe75b0d5a46) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `spreadsheet.json test fixture mismatch: Zod v4 serializes union as type array instead of anyOf`
- 10 min: `ReferenceError: crypto is not defined in Node 18 CJS when MCP SDK calls crypto.randomUUID()`
- `SSE multi-client test failed with 404 (cascade from streamable crash leaving port occupied)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
