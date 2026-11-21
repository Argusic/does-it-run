# saq

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/tobymao/saq, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/saq

## Pinned environment

- Project commit: `525acc9251c95395b14090ebe481dac6a79062a5`
- Test commit: `525acc9251c95395b14090ebe481dac6a79062a5`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 7.9 to 12.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 7.9 | 3 | 3 | [run](https://argusic.com/run/8512e621-be00-4764-8361-fdc3422eb6ed) |
| 2 | pass | 100 | 30 | 12.7 | 3 | 3 | [run](https://argusic.com/run/1d9e1089-41db-4553-b901-b731afa2b988) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `pip install -e '.[hiredis,web,dev,redis,postgres]' failed: externally-managed-environment (PEP 668)`
- 1 min: `PostgreSQL ./configure failed: ICU not found`
- 5 min: `psycopg ImportError: no pq wrapper available, libpq library not found at runtime`

Attempt 2:

- 1 min: `PostgreSQL library libpq not found, psycopg backend failed to load`
- 1 min: `pip install failed due to externally-managed-environment (PEP 668)`
- 10 min: `Docker not available to start Redis and Postgres containers`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
