# onedump

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/liweiyi88/onedump, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/onedump

## Pinned environment

- Project commit: `7d4e2bd7d316d64746814c1a9a130bf83315908e`
- Test commit: `7d4e2bd7d316d64746814c1a9a130bf83315908e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 10.8 to 10.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 10.8 | 3 | 3 | [run](https://argusic.com/run/a91ae492-9a36-4035-9144-d65bcdcb692e) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `go not found in PATH`
- 1 min: `google.golang.org/grpc v1.72.2 incompatible with Go 1.27 (undefined: http2.TrailerPrefix)`
- 1 min: `mysqldump not found; pg_dump not found; mysqlbinlog not found; mysql not found`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
