# cms

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/bcms/cms, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/cms

## Pinned environment

- Project commit: `d0e643d3269c27f20f57b23dfed4b45655a465fb`
- Test commit: `d0e643d3269c27f20f57b23dfed4b45655a465fb`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 12.2 to 12.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 10 | 12.2 | 4 | 4 | [run](https://argusic.com/run/2e85ec4e-2b07-4970-998e-55f0f7868ebf) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Node.js v18 installed but project requires Node.js 20`
- 1 min: `Docker not available in container, cannot use docker compose up`
- 2 min: `No MongoDB instance available`
- 1 min: `mongodb-memory-server URI had no database name, causing @fastify/mongodb to not set fastify.mongo.db`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
