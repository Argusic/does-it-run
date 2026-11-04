# pgcli

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/dbcli/pgcli, licensed BSD-3-Clause, written in Python.

Evidence and recordings: https://argusic.com/subject/pgcli

## Pinned environment

- Project commit: `101e523eb2987ada87231c4533f0ab701c4c3124`
- Test commit: `101e523eb2987ada87231c4533f0ab701c4c3124`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 2.7 to 5.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 5.2 | 3 | 3 | [run](https://argusic.com/run/bdc55d40-7f1e-46e1-bd18-539642adfb34) |
| 2 | pass with mocks | 92 | 0.5 | 2.7 | 1 | 1 | [run](https://argusic.com/run/a73243d5-7c34-4aaf-be9d-65a063ffadfe) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `pip install failed due to externally-managed-environment (PEP 668)`
- 1 min: `psycopg requires system libpq which is not installed and can't be apt-installed (no root)`
- 3 min: `No PostgreSQL server available to run database-dependent tests`

Attempt 2:

- 1.5 min: `psycopg-binary required: imported psycopg (source) but libpq not found in system; venv pip install missing psycopg-binary for bundled libpq`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
