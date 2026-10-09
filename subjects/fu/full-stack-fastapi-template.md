# full-stack-fastapi-template

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/fastapi/full-stack-fastapi-template, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/full-stack-fastapi-template

## Pinned environment

- Project commit: `f27b4721507824e57ebd0286ff1a84d82e83bf59`
- Test commit: `f27b4721507824e57ebd0286ff1a84d82e83bf59`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 7.1 to 7.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3.5 | 7.1 | 4 | 4 | [run](https://argusic.com/run/912dadce-7353-4e30-b4c6-282355003438) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `uv not in PATH; Python 3.14 not available`
- 0.5 min: `Frontend directory backend/app/frontend missing (app.frontend() on startup)`
- 3 min: `PostgreSQL not installed; no psql, pg_ctl, initdb, or libpq system libraries`
- 0.5 min: `Alembic migrations not applied to database`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
