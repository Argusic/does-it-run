# payload

**Verdict: runs.** Argusic Score 80 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/payloadcms/payload, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/payload

## Pinned environment

- Project commit: `72ee1751b153bd1cf9e44a7fad85563fa3f57b4e`
- Test commit: `72ee1751b153bd1cf9e44a7fad85563fa3f57b4e`
- Worker image digests: `sha256:33ceb71981b602c1a7443a53469e4dba065f7503eab3078a2d7a57a2ab987517`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services, real run
- Valid runs: 5; wall time 6.2 to 58.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 50 | 4 | 6.2 | 4 | 4 | [run](https://argusic.com/run/89707f97-4848-470b-a577-b2ce5d62ea31) |
| 1 | fail | 50 | 3 | 32.3 | 3 | 3 | [run](https://argusic.com/run/1e916a6f-ead1-42b6-a6b5-1d6d1a0645b5) |
| 2 | pass | 100 | 7 | 20.5 | 4 | 4 | [run](https://argusic.com/run/515d551f-f630-4fae-89f0-d95dc66dd4e4) |
| 2 | pass | 100 | 13 | 13.7 | 2 | 2 | [run](https://argusic.com/run/022275ff-20e3-4cb2-b37b-7602e58c029a) |
| 3 | pass | 100 | 57 | 58.1 | 7 | 7 | [run](https://argusic.com/run/2b307a38-0089-4de9-84c7-bea4cdede82f) |

## What was observed on a clean machine

Attempt 1:

- `Node.js version mismatch: project requires >=24.15.0, container has v18.19.1`
- `file-type@22.0.1 uses regex /\d+/v flag (Node 20+ feature) not available in Node 18`
- `Test commands require --no-experimental-strip-types flag (Node 24+ feature)`
- `rollup-plugin-dts fails to initialize TypeScript compiler`

Attempt 1:

- 0.5 min: `packages/next/bundleWithPayload.js uses import.meta.dirname (Node 21+)`
- 1.5 min: `file-type@22.0.1 uses v-flag regex (Node 20+), blocks all tests and dev server`
- `html-encoding-sniffer@6 require()s ESM-only @exodus/bytes (Node 18+ERR_REQUIRE_ESM)`

Attempt 2:

- 1 min: `Node.js v18.19.1 installed but project requires v24.15.0`
- `pnpm 11.9.0 requires Node 22+ but only Node 18 available`
- 1 min: `MongoDB not available at localhost:27018`
- 2 min: `JavaScript heap out of memory during build`

Attempt 2:

- 2 min: `rollup-plugin-dts@6.2.3 incompatible with TypeScript 7.0.2 (Cannot read properties of undefined 'useCaseSensitiveFileNames')`
- 3 min: `Node.js v18.19.1 lacks ReadableStream.from() and /v regex flag, causing test failures`

Attempt 3:

- 1 min: `pnpm not available globally - EACCES on /usr/local/lib/node_modules`
- 3 min: `rollup-plugin-dts resolved to TypeScript 7.0.2 instead of TS6 compatibility layer`
- 1 min: `rollup bundle:types ran out of memory on Node 18 (FATAL ERROR: Ineffective mark-compacts)`
- 2 min: `import.meta.dirname not supported in Node 18`
- 3 min: `Node 18.19.1 did not meet project requirement of >=24.15.0`
- 2 min: `better-sqlite3 native module failed to load with Node 24`
- 1 min: `pnpm vitest invoked create-payload-app CLI instead of vitest with Node 24`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
