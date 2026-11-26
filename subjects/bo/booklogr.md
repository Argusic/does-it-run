# booklogr

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Mozzo1000/booklogr, licensed Apache-2.0, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/booklogr

## Pinned environment

- Project commit: `af82e44c220f02ba6d7bfb89b8c4b040ea554550`
- Test commit: `af82e44c220f02ba6d7bfb89b8c4b040ea554550`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 10.4 to 10.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 15 | 10.6 | 3 | 3 | [run](https://argusic.com/run/69e284c6-2934-461e-8d6a-45337699077f) |
| 2 | pass | 100 | 9 | 10.4 | 3 | 3 | [run](https://argusic.com/run/ad3a4fed-dfe2-4d63-90b0-8461d390dc6d) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `psycopg2 build fails: pg_config not found`
- 1 min: `load_dotenv() called after api imports; Config class reads env vars at class-definition time`
- 5 min: `No database tables; instance path mismatch between flask db upgrade and runtime`

Attempt 2:

- 2 min: `psycopg2 package requires libpq-dev (pg_config not found), fails to build from source`
- 3 min: `Node.js v18.19.1 too old for Vite 8 (requires 20.19+) - ReferenceError: CustomEvent is not defined`
- 2 min: `gunicorn workers crash on startup because Config.alert() fires when AUTH_SECRET_KEY not yet set; load_dotenv() in app.py runs after Config class is evaluated`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
