# fastmcp

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/punkpeye/fastmcp, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/run/46793793-3603-458f-a485-0801524f81f3

## Pinned environment

- Project commit: `915cc605988e1179ce2568d82443a3af77825f39`
- Test commit: `915cc605988e1179ce2568d82443a3af77825f39`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 56.9 to 56.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 52 | 56.9 | 5 | 5 | [run](https://argusic.com/run/46793793-3603-458f-a485-0801524f81f3) |

## What was observed on a clean machine

Attempt 1:

- 7 min: `36 edge transport tests fail: ReferenceError: crypto is not defined`
- 1 min: `pnpm install blocked by ERR_PNPM_IGNORED_BUILDS (esbuild, tldjs)`
- `openapi/loadSpec.test.ts and fromOpenAPI.offline.test.ts fail with ERR_REQUIRE_ESM`
- `SSE-dependent tests in FastMCP.test.ts, FastMCP.batch-methods.test.ts, FastMCP.ext-apps.test.ts, FastMCP.sse-auth.test.ts, FastMCP.oauth-no-store.test.ts, FastMCP.oauth-proxy.test.ts, FastMCP.oauth-body-reader.test.ts, FastMCP.routes.test.t`
- `CLI binary (dist/bin/fastmcp.js) requires Node 20+ (yargs-parser min version)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
