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
- Valid runs: 2; wall time 37.8 to 44.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 37 | 37.8 | 3 | 3 | [run](https://argusic.com/run/3c481f48-dc51-45c8-a930-efe75b0d5a46) |
| 2 | pass | 100 | 47 | 44.6 | 2 | 2 | [run](https://argusic.com/run/6093a4b2-6c7b-4443-a06e-35df63f6c04f) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `spreadsheet.json test fixture mismatch: Zod v4 serializes union as type array instead of anyOf`
- 10 min: `ReferenceError: crypto is not defined in Node 18 CJS when MCP SDK calls crypto.randomUUID()`
- `SSE multi-client test failed with 404 (cascade from streamable crash leaving port occupied)`

Attempt 2:

- 47 min: `npm run build emitted a 43-test suite that failed (39/43) out of the box in this container (Node 18.19.1): SDK 1.32.x streamable transport threw ReferenceError: crypto is not defined, and zod 4.6.7's union-to-JSON-Schema compaction broke th`
- 20 min: `SSE with multiple clients failed reliably when run after the streamable test (SSE error Non-200 status code 404) because the crashing streamable server held port 1122`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
