# cassandra-nodejs-driver

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/apache/cassandra-nodejs-driver, licensed Apache-2.0, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/cassandra-nodejs-driver

## Pinned environment

- Project commit: `4620e5417e7de2fc0dc3d31c683cb028b484092f`
- Test commit: `4620e5417e7de2fc0dc3d31c683cb028b484092f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 1.2 to 13 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 0.5 | 1.2 | 1 | 1 | [run](https://argusic.com/run/66ad8bc7-791a-4f86-a76f-6dfd0b30d32f) |
| 2 | pass | 100 | 0.5 | 13 | 2 | 2 | [run](https://argusic.com/run/2be3eeb8-530f-4a6e-8379-ba52fdd8749b) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `Node.js v18.19.1 installed but project requires >=20`

Attempt 2:

- `Node.js v18.19.1 is below the required >=20`
- 8 min: `2 insights-client tests failed due to timing - async init chain (fs.readFile in _getAppInfo) took ~30ms before scheduling timers, but test check windows (60ms/20ms) fired before status event timer could execute`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
