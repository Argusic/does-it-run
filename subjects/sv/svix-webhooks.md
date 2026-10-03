# svix-webhooks

**Verdict: runs with mocks.** Argusic Score 71 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/svix/svix-webhooks, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/svix-webhooks

## Pinned environment

- Project commit: `cb056ba1a92a1fa1f812011354825dae81905fba`
- Test commit: `cb056ba1a92a1fa1f812011354825dae81905fba`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 13 to 21.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 50 | 6.1 | 21.9 | 2 | 2 | [run](https://argusic.com/run/18a07446-7d38-444d-ab8f-8978570a7a3a) |
| 2 | pass with mocks | 92 | 3 | 13 | 3 | 3 | [run](https://argusic.com/run/fe0fc990-e30f-484c-bbdb-bfd72a0633fc) |

## What was observed on a clean machine

Attempt 1:

- 1.5 min: `test_cache_or_queue_dsn_priority panics because load().unwrap() requires env vars SVIX_JWT_SECRET and SVIX_REDIS_DSN when queue_type=redis`
- 1 min: `JavaScript library cannot build with Node 18.19.1 (requires >=22)`

Attempt 2:

- 2 min: `JavaScript library build fails on Node 18: tsdown bundler requires 'styleText' from 'node:util' which is only available in Node >=21`
- 1 min: `Python test_openapi_json_is_available requires docker-compose which is not installed in this environment`
- 1 min: `JavaScript tests fail: mockttp depends on get-port (ESM-only) but test runner uses require() in CJS mode, Node 18 doesn't support dynamic import for ESM modules in CJS`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
