# percona-backup-mongodb

**Verdict: runs with mocks.** Argusic Score 85.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/percona/percona-backup-mongodb, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/percona-backup-mongodb

## Pinned environment

- Project commit: `f007d41c07149099e422ed9479575ba3dc01ab45`
- Test commit: `f007d41c07149099e422ed9479575ba3dc01ab45`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 8.1 to 8.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 85.33 | 2 | 8.1 | 3 | 2 | [run](https://argusic.com/run/9bd900b8-ae44-475c-a31f-ca4d827eb4ee) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `go binary not on PATH`
- 1 min: `Makefile hardcodes -tags gssapi but krb5-dev headers not installable without root`
- `Docker not installed; 10 pbm test packages and 3 x/ test packages require docker containers (mongodb, etcd, minio, gcs)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
