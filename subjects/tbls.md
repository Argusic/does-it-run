# tbls

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/k1LoW/tbls, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/tbls

## Pinned environment

- Project commit: `188868990583ac27ad26ac3617f0a62233075ed6`
- Test commit: `188868990583ac27ad26ac3617f0a62233075ed6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 44.3 to 44.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 44 | 44.3 | 4 | 4 | [run](https://argusic.com/run/74ed87b1-ca60-4f4d-8e4e-21bb2db8b334) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `Go 1.27.1 compiler not found in container`
- 8 min: `First build without -tags sqlite_fts5 hit 'no such module: fts5'`
- `Datasource test requires MySQL/Postgres/MSSQL servers (connection refused)`
- `sqlite3 CLI binary not installed`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
