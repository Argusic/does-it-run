# pg_net

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/supabase/pg_net, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/pg-net

## Pinned environment

- Project commit: `5fb36dd982bc34988d73bdea07ff66795a4e35ba`
- Test commit: `5fb36dd982bc34988d73bdea07ff66795a4e35ba`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 25.7 to 33 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 33 | 0 | 0 | [run](https://argusic.com/run/f9034dd6-d612-4bd5-bb1f-5ff5e8e82faf) |
| 2 | pass | 100 | 35 | 25.7 | 7 | 7 | [run](https://argusic.com/run/1eb5bf9c-bda0-43cc-990a-45bd19a65c05) |

## What was observed on a clean machine

Attempt 2:

- 5 min: `make link failed: cannot find -lcurl (no curl dev package installed)`
- 4 min: `postgres startup failed: could not access file pg_stat_statements`
- 2 min: `pg_net background worker crashed: role "" does not exist`
- 3 min: `pip install blocked by PEP 668 and psycopg import failed`
- 3 min: `tests could not connect: default socket path not writable and roles missing`
- 8 min: `nginx failed: unknown directive if/echo and missing PCRE/zlib`
- 10 min: `partial-suite runs failed on leftover state (orphaned net schema, stale queue rows, pre-created pg_stat_statements/roles)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
