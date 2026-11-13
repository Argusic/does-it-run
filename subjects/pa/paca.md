# paca

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Paca-AI/paca, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/paca

## Pinned environment

- Project commit: `839c532ca45183db136569de55cdf5fae4e3fd40`
- Test commit: `839c532ca45183db136569de55cdf5fae4e3fd40`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 6.4 to 9.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 28 | 6.4 | 5 | 5 | [run](https://argusic.com/run/8b0227ad-515f-4583-b621-0ba435d3f81b) |
| 2 | pass | 100 | 3 | 9.8 | 5 | 5 | [run](https://argusic.com/run/13e2f688-0cb8-4b98-a75e-b253c2185b49) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `npm install failed with 'Cannot read properties of null (reading edgesOut)' , Arborist peer dependency resolution crash on Node 18`
- 6 min: `jsdom@29.1.1's html-encoding-sniffer dep uses require() on @exodus/bytes (ESM-only), which throws ERR_REQUIRE_ESM on Node 18`
- 3 min: `vitest@4.x uses rolldown which imports from node:util (Node 22+ only), crashing on startup`
- 5 min: `@blocknote/core/dist uses Array.toReversed() (Node 22+ API) , crashes with 'not a function or its return value is not iterable'`
- `apps/web: @tailwindcss/oxide-linux-x64-gnu native binding missing , npm optional dep resolution bug on this platform`

Attempt 2:

- 3 min: `Node.js v18.19.1 is too old for vitest 4.x (needs node:util.styleText from Node >=22). Resolution: installed nvm and Node.js v22.23.5.`
- 1 min: `npm v9.2.0 cannot resolve dependency tree in apps/mcp (elevateError: Cannot read properties of null). Resolution: used nvm's npm v10.9.9 with --legacy-peer-deps.`
- 1 min: `Rolldown native binding missing when vitest ran with old node_modules built under Node 18. Resolution: reinstalled node_modules with Node 22.`
- 1 min: `Go toolchain not installed. Resolution: downloaded Go 1.23.4 binary tarball.`
- 1 min: `Unzip not installed; cannot install Bun for services/realtime.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
