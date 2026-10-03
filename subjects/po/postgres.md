# postgres

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/porsager/postgres, licensed Unlicense, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/postgres

## Pinned environment

- Project commit: `411429e7bd7a3d61155ca9a70a97c111823702ea`
- Test commit: `411429e7bd7a3d61155ca9a70a97c111823702ea`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 15.4 to 15.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 15.4 | 6 | 6 | [run](https://argusic.com/run/7c02faaf-0cf5-486f-a76e-cebb062024fd) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `PostgreSQL server not installed in container`
- 2 min: `bootstrap.js references /var/run/postgresql socket not available without root`
- 1 min: `Default pg_hba.conf had trust for all, causing auth-failure test to pass incorrectly`
- 1 min: `Prepared transactions disabled (default), subscribe requires wal_level=logical`
- 1 min: `SSL test failed because PGHOST=/tmp forced Unix socket connections instead of TCP`
- `deno binary not available in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
