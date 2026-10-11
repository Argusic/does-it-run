# sensu-go

**Verdict: runs.** Argusic Score 93.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/sensu/sensu-go, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/sensu-go

## Pinned environment

- Project commit: `80e82590ece98a4bc780de04882a6f754ad12abc`
- Test commit: `80e82590ece98a4bc780de04882a6f754ad12abc`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 17.7 to 17.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 93.33 | 17 | 17.7 | 3 | 2 | [run](https://argusic.com/run/c78b1893-9d5a-4d2d-a761-1a3b371462c0) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Go toolchain not installed in container`
- 3 min: `PostgreSQL not installed; sensu-backend requires a PostgreSQL store`
- 2 min: `Pre-existing test failure TestLegacyAdapter_GH4675 in backend/pipeline/handler; timing-dependent test consistently fails on Go 1.18 and Go 1.22`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
