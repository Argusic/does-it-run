# twurple

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/twurple/twurple, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/twurple

## Pinned environment

- Project commit: `c487a28ae1e9e76c59dc085a52fbe6242e16d45b`
- Test commit: `c487a28ae1e9e76c59dc085a52fbe6242e16d45b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 6.3 to 6.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 7 | 6.3 | 3 | 3 | [run](https://argusic.com/run/49b690f5-6b8d-4dcc-9abc-f675073c8cab) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `npm install crashed: Cannot read properties of null (reading 'edgesOut') on bundled npm 9 + Node 18 (vitest 4 needs Node 20)`
- 3 min: `Same arborist edgesOut crash after Node upgrade due to unpinned vitest ^4.0.13 resolving to interdependent 4.1.11/@vitejs/devtools peer ranges`
- 1 min: `E2E exercise script used nonexistent method and first mock lacked query-aware users route, so unknown-user assertion failed`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
