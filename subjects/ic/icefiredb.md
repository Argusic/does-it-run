# IceFireDB

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/IceFireDB/IceFireDB, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/icefiredb

## Pinned environment

- Project commit: `c2a6335930e3226d8bc5a5b53951c75ece586c0f`
- Test commit: `c2a6335930e3226d8bc5a5b53951c75ece586c0f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 9.8 to 11.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 11.7 | 0 | 0 | [run](https://argusic.com/run/9296a8e6-9c18-4c5a-9159-988ea0b673aa) |
| 2 | pass | 100 | 2.5 | 9.8 | 2 | 2 | [run](https://argusic.com/run/b274be76-9143-49a1-bb4d-d1c28a2d1778) |

## What was observed on a clean machine

Attempt 2:

- 1.5 min: `Vendor directory missing IceFireDB/ package sources (icefiredb-crdt-kv, icefiredb-ipfs-log) causing build failures with -mod=vendor`
- `Missing .env file causes main.go warning log`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
