# wikipedia-semantic-search

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/upstash/wikipedia-semantic-search, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/wikipedia-semantic-search

## Pinned environment

- Project commit: `e0bad8f0c256cee13377dc861f9fd7b16018d9c9`
- Test commit: `e0bad8f0c256cee13377dc861f9fd7b16018d9c9`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 30 to 30 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 30 | 30 | 5 | 5 | [run](https://argusic.com/run/36a9fddb-a2cc-461e-90e9-24137fb71426) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `pnpm not installed in container (no root)`
- 5 min: `next build failed during page data collection: UPSTASH_VECTOR_REST_TOKEN is missing (env not configured)`
- 8 min: `production next start exited after .next lost BUILD_ID following a dev run; first start with mock env also died at container exec teardown`
- 15 min: `mock-only: chat endpoint returned 500 because history pipeline needed list semantics (pipeline result array) and vector query mock routing/response shape were incomplete; later the mock LLM was bypassed by the app hardcoding https://api.ope`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
