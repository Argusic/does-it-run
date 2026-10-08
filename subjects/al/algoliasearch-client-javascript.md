# algoliasearch-client-javascript

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/algolia/algoliasearch-client-javascript, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/algoliasearch-client-javascript

## Pinned environment

- Project commit: `e44ad251243f8c86413c34e9b49c0a0d40f14710`
- Test commit: `e44ad251243f8c86413c34e9b49c0a0d40f14710`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 31.3 to 31.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 31 | 31.3 | 3 | 3 | [run](https://argusic.com/run/4276758f-1576-4b3b-a6c2-cd8432042d88) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `yarn not found in container`
- 4 min: `Node v18.19.1 too old (required v24.21.0 per .nvmrc), vitest/rolldown could not start`
- 18 min: `Build failed because dependent packages not pre-built (no DTS files in client-*, ingestion, monitoring etc.)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
