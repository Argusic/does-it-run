# FerretDB

**Verdict: could not verify.** Argusic Score 80 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/FerretDB/FerretDB, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/ferretdb

## Pinned environment

- Project commit: `799235dab9e350655e72e65a0b24d849f7d68143`
- Test commit: `799235dab9e350655e72e65a0b24d849f7d68143`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 2; wall time 9.8 to 11.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 3.2 | 9.8 | 5 | 5 | [run](https://argusic.com/run/fd33bd1a-04d0-4cb8-9133-2e1f0a0e2d4a) |
| 2 | fail | 80 | 9 | 11.1 | 5 | 5 | [run](https://argusic.com/run/81d9f3a3-1fef-47c6-a770-ab76a443c35e) |

## What was observed on a clean machine

Attempt 1:

- 2.5 min: `Go 1.25 not installed`
- 1 min: `git describe failed , no annotated tags`
- 0.5 min: `resource test flaky without ferretdb_dev tag`
- 0.5 min: `build/version test failed , commit.txt missing`
- 0.2 min: `PostgreSQL-dependent tests fail without database`

Attempt 2:

- 1 min: `Go not pre-installed in container`
- 1 min: `build/version/version.txt and related files missing (no git tags)`
- 1 min: `cmd/ferretdb/ test failed: bin/ferretdb binary not found`
- 1 min: `resource test TestTrackUntrack/LocalCleanup failed without ferretdb_dev tag`
- `All tests requiring PostgreSQL with DocumentDB extension fail: internal/documentdb, internal/dataapi, ferretdb , no PostgreSQL installed and no root/Docker access`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
