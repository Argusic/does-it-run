# editor

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/playcanvas/editor, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/editor

## Pinned environment

- Project commit: `01748332fa5c26c91c1574d8f3d7dd058ed74e92`
- Test commit: `01748332fa5c26c91c1574d8f3d7dd058ed74e92`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 4.9 to 4.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 4 | 4.9 | 3 | 3 | [run](https://argusic.com/run/95555d7a-2702-4020-a652-ee4c733ea26a) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Node 18 cannot run the project (mocha 12/vite 7 need >=20.19/22.12); npm test crashed with 'Unexpected token 'with''`
- 2 min: `npm run typecheck fails with pre-existing errors (code-editor PCUI type mismatches)`
- 4 min: `Browser-based E2E suite and UI launch cannot run: no browser engine or Docker in container, and suite requires real PlayCanvas login cookies (PC_COOKIE_VALUE)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
