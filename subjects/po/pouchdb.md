# pouchdb

**Verdict: runs.** Argusic Score 96.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/apache/pouchdb, licensed Apache-2.0, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/pouchdb

## Pinned environment

- Project commit: `27de91f1105a8074ddd06f5a23156dd99c4eb016`
- Test commit: `27de91f1105a8074ddd06f5a23156dd99c4eb016`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 4.4 to 6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.25 | 4.4 | 1 | 1 | [run](https://argusic.com/run/3f10e5ee-2628-4ade-9af8-ec742c861129) |
| 2 | pass | 93.33 | 0.5 | 6 | 3 | 2 | [run](https://argusic.com/run/3fa7c0f1-cc20-4372-b70e-f37552adeb8a) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `URL.parse is not a function on Node.js 18`

Attempt 2:

- 0.2 min: `npm run test-unit exited 1 before a build: Cannot find module packages/node_modules/pouchdb-for-coverage/lib/index.js`
- 2 min: `npm test failed the HTTP adapter with TypeError: URL.parse is not a function because Node 18's global URL has no parse method`
- 2 min: `The first full BAIL=0 run had one failing test: test.issue3179.js-local-http non-live sync found no expected conflict, with 1,932 passing, 42 pending, and 1 failing`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
