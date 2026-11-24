# agentos

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/framerslab/agentos, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/agentos

## Pinned environment

- Project commit: `fa3ec4a47f8521026e8c10aa876d082152b289d8`
- Test commit: `fa3ec4a47f8521026e8c10aa876d082152b289d8`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 41.1 to 54.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 54.3 | 5 | 5 | [run](https://argusic.com/run/bf35b531-758b-4f99-b672-efef907efe56) |
| 2 | pass with mocks | 92 | 41 | 41.1 | 3 | 3 | [run](https://argusic.com/run/d2112d83-b2d3-493b-8a33-88850529a6cf) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `pnpm install failed with ERR_PNPM_IGNORED_BUILDS: pnpm-workspace.yaml had invalid YAML syntax (string instead of YAML list)`
- 8 min: `hnswlib-node native addon binary not found (build script was blocked)`
- 1 min: `better-sqlite3 native addon binary not found; FTS5 full-text search engine unavailable causing 7 memory tests to fail`
- 3 min: `crypto.randomUUID() not available as global in vitest's Node.js 18 execution context, causing 25+ tests to throw ReferenceError`
- 1 min: `generateText unit test regex did not match actual error message '[400] invalid is not a valid model ID'`

Attempt 2:

- 2 min: `TypeScript build error: FinalizationRegistry type mismatch in Brain.ts and MemoryStore.ts - custom FinalizerLike interface declared unregister() returning boolean but Node 18's TS lib returns void`
- 5 min: `Runtime test failures: crypto is not defined - 8 source files used crypto.randomUUID() without importing from node:crypto`
- 1 min: `Missing graphology dependency causing CapabilityGraph and discovery tests to fail`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
