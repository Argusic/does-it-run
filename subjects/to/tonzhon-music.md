# tonzhon-music

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/enzeberg/tonzhon-music, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/tonzhon-music

## Pinned environment

- Project commit: `764bd60c60c55c3609f9183d15aa3fb85711652d`
- Test commit: `764bd60c60c55c3609f9183d15aa3fb85711652d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 4.6 to 8.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 6 | 8.3 | 4 | 4 | [run](https://argusic.com/run/2490bb66-51cc-4b63-b012-c7f1036ea033) |
| 2 | pass with mocks | 92 | 22 | 4.6 | 6 | 6 | [run](https://argusic.com/run/56264d71-a72a-4e30-9728-97cd0a1e8b3c) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Node.js v18 too old (needs >=20.19)`
- 1 min: `@rolldown/binding-linux-x64-gnu native binding missing (npm install ran under Node 18)`
- 1 min: `manualChunks object type not supported by Vite 8/rolldown (must be function)`
- 5 min: `Backend API host tonzhon.whamon.com does not resolve in DNS`

Attempt 2:

- 2 min: `Node.js v18.19.1 too old for Vite 8 (requires >=20.19 or >=22.12)`
- 1 min: `npm install with old Node left broken native bindings for @rolldown/binding`
- 1 min: `vite.config.js loaded as CommonJS but uses ESM syntax`
- 2 min: `manualChunks config as object rejected by Rolldown in Vite 8`
- 1 min: `__dirname not supported by Vite 8 native config loader`
- 5 min: `Real backend tonzhon.whamon.com unreachable`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
