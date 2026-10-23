# nebula

**Verdict: runs.** Argusic Score 82.5 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/dennis-tra/nebula, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/run/eac200e7-9f51-481e-b3ff-909d62a633ef

## Pinned environment

- Project commit: `25b61219e5cae64fd85160d710375c1b67b1065f`
- Test commit: `25b61219e5cae64fd85160d710375c1b67b1065f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 7.2 to 15.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 65 | 5 | 7.2 | 4 | 1 | [run](https://argusic.com/run/eac200e7-9f51-481e-b3ff-909d62a633ef) |
| 2 | pass | 100 | 15 | 15.8 | 3 | 3 | [run](https://argusic.com/run/ba99dc27-d232-4339-bee5-7aad64eef3eb) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Go 1.23.2 not installed in container`
- `DB tests fail: no PostgreSQL or ClickHouse (no Docker)`
- `maxmind tests fail: missing GeoLite2-ASN.mmdb and GeoLite2-Country.mmdb`
- `udger test skipped: missing Udger DB file`

Attempt 2:

- 3 min: `Go compiler not pre-installed in container`
- 10 min: `Docker not available; README test recipe (just test) requires Docker containers for Postgres and ClickHouse databases`
- 2 min: `ClickHouse tests failed due to timezone location mismatch: expected time.UTC vs actual time.Location("Etc/UTC")`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
