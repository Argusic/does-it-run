# eko

**Verdict: runs with mocks.** Argusic Score 80 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/FellouAI/eko, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/eko

## Pinned environment

- Project commit: `c3de315af2c178826f8b1682b52638d18131252d`
- Test commit: `c3de315af2c178826f8b1682b52638d18131252d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 8.2 to 27.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 7 | 8.2 | 5 | 5 | [run](https://argusic.com/run/695131be-17c3-4a66-b8d6-f7faf72fd399) |
| 2 | pass with mocks | 80 | 12 | 27.3 | 5 | 2 | [run](https://argusic.com/run/9ca87832-ef93-4752-992b-f43d3c968777) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `pnpm not pre-installed in container`
- 2 min: `pnpm install blocked 8 build scripts (canvas, classic-level, core-js, keytar, leveldown, sqlite3, tldjs)`
- 1 min: `pnpm -r --sequential build flag unsupported in pnpm 12`
- `eko-nodejs and example/nodejs require Node.js 20+ (Playwright dependency)`
- `11 of 14 test suites require real LLM API keys`

Attempt 2:

- 2 min: `pnpm build uses '--sequential' flag unsupported by pnpm 12.8.1`
- `test/llm/utils.test.ts: call_timeout with 200ms timeout on a 300ms async function rejects with Timeout but the test does not catch the rejected promise (pre-existing bug in the test itself)`
- `test/llm/mcp.test.ts: requires an external MCP SSE server at http://localhost:8083 (integration test, cannot mock)`
- `eko-nodejs test/mcp.test.ts: Playwright requires Node.js 20+, container has 18.19.1`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
