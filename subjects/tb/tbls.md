# tbls

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/k1LoW/tbls, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/tbls

## Pinned environment

- Project commit: `188868990583ac27ad26ac3617f0a62233075ed6`
- Test commit: `188868990583ac27ad26ac3617f0a62233075ed6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 11.9 to 44.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 44 | 44.3 | 4 | 4 | [run](https://argusic.com/run/74ed87b1-ca60-4f4d-8e4e-21bb2db8b334) |
| 2 | pass | 100 | 12 | 11.9 | 3 | 3 | [run](https://argusic.com/run/5f151bab-1d59-4dea-8344-4e885d3e29ea) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `Go 1.27.1 compiler not found in container`
- 8 min: `First build without -tags sqlite_fts5 hit 'no such module: fts5'`
- `Datasource test requires MySQL/Postgres/MSSQL servers (connection refused)`
- `sqlite3 CLI binary not installed`

Attempt 2:

- 3 min: `Go not installed in container; required go1.25.8 per toolchain directive`
- 1 min: `sqlite3 CLI not available; Makefile target for test DB creation fails`
- 2 min: `datasource tests fail with connection refused on mysql:33306, pg:55432, mssql:11433 (no DB servers running)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
