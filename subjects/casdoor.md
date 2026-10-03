# casdoor

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/casdoor/casdoor, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/casdoor

## Pinned environment

- Project commit: `0f7d6842f23fdf14f3c88df9cf842a940983a45d`
- Test commit: `0f7d6842f23fdf14f3c88df9cf842a940983a45d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 13.9 to 13.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 16 | 13.9 | 9 | 9 | [run](https://argusic.com/run/930bf01f-626c-4128-8b98-a6b4965c2012) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go compiler not found in container`
- 1 min: `conf/app.conf configured for MySQL but no MySQL server available`
- 2 min: `init_data.json does not exist (only template exists)`
- 1 min: `CreateDatabase() runs CREATE DATABASE IF NOT EXISTS which SQLite does not support`
- 1 min: `Frontend yarn install fails on Node 18 due to eslint-visitor-keys engine requirement >=20.19`
- `util.TestGetVersion fails - requires specific git history (v1.257.0 tag)`
- `certificate.TestGetClient fails - missing acme_account.key fixture`
- `xlsx.TestReadSheet fails - missing tmpFiles/example fixture`
- `object.TestGetUsers panics with index out of range - test expects DB with data`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
