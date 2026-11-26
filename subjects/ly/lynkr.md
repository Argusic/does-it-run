# Lynkr

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Fast-Editor/Lynkr, licensed Apache-2.0, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/lynkr

## Pinned environment

- Project commit: `24f5c602fe6813fe85d66277d18d0b5479bd2af3`
- Test commit: `24f5c602fe6813fe85d66277d18d0b5479bd2af3`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 31 to 39.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 2 | 31 | 6 | 6 | [run](https://argusic.com/run/617dc971-5c2e-4ad3-847d-e9bde48c8d91) |
| 2 | pass with mocks | 92 | 35 | 39.5 | 6 | 6 | [run](https://argusic.com/run/3e2bfa7d-aae7-4579-8592-ef70e407365f) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Config requires DATABRICKS_API_BASE and DATABRICKS_API_KEY before starting the proxy or loading config modules`
- 3 min: `better-sqlite3 optional native dependency not compiled for Node 18 (npm install skipped binary build)`
- 3 min: `task-ledger test suite cascading failure: Promise resolution is still pending , t.unref() on setTimeout in Node 18 causes event loop to exit before timer fires`
- 1 min: `jev-router.test.js classifyJev LRU test fails because evaluateJev requires TYPESAFE_API_KEY`
- 1 min: `jev-routing.test.js scoreIntent test fails because classifyJev requires TYPESAFE_API_KEY`
- 1 min: `tencentdb-launcher.test.js expects tencentdbMemory.enabled defaults to true but code defaults to false (TENCENTDB_MEMORY_ENABLED === 'true')`

Attempt 2:

- 20 min: `Node.js v18.19.1 (package requires >=20) , better-sqlite3 optional dep couldn't be installed via npm due to missing prebuilt binaries`
- `session-affinity test: read-through recovers a pin from SQLite when memory is cleared failed , telemetry.getDb() returned null because better-sqlite3 wasn't loadable`
- 4 min: `routing-propensity test: static path expected provider=databricks but got ollama , dotenv.config() set MODEL_PROVIDER=.env before test body overrode it`
- 4 min: `session-fingerprint test: force-cloud with tier routing used tier_config instead of force , FALLBACK_ENABLED=false from .env made isFallbackEnabled() return false, skipping force_cloud branch`
- 2 min: `jev-router LRU test: classifyJev returned null because getApiKey() needs TYPESAFE_API_KEY env var , not set in .env or test harness`
- 2 min: `task-ledger test: 3 subtests cancelledByParent due to Node 18 async event loop issue with never-resolving promise in timeout/null test`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
