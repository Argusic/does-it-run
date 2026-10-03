# autoflow

**Verdict: could not verify.** Argusic Score 25 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/pingcap/autoflow, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/autoflow

## Pinned environment

- Project commit: `c4cb19d8fa205bdd4cb38d0ac250d273fcc3e5f2`
- Test commit: `c4cb19d8fa205bdd4cb38d0ac250d273fcc3e5f2`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 2; wall time 24.4 to 29.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 30 | 3 | 24.4 | 4 | 0 | [run](https://argusic.com/run/c176f961-b33a-4df1-93d7-3ff385ad68b5) |
| 2 | fail | 20 | n/a | 29.5 | 0 | 0 | [run](https://argusic.com/run/7fdcec64-1ef5-4f5b-82cb-7bd6085f2baf) |

## What was observed on a clean machine

Attempt 1:

- 15 min: `TiDB/MySQL server required , backend engine connects to localhost:4000 on module import; no Docker and no root to install MySQL/TiDB`
- 5 min: `No Redis server , required by Celery/Flower for async task queue, cannot start full backend`
- 10 min: `Backend lifespan startup fails , engine.connect() raises OperationalError (2003) to localhost:4000; 138 routes import but server cannot bind`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
