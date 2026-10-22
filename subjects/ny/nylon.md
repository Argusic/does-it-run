# nylon

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/encodeous/nylon, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/nylon

## Pinned environment

- Project commit: `93ad8733c75bcfd545e6e4fd91132bad7b979a88`
- Test commit: `93ad8733c75bcfd545e6e4fd91132bad7b979a88`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 11.9 to 22.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 11.9 | 0 | 0 | [run](https://argusic.com/run/253c1ee6-6c90-4010-b049-b9909a8e102c) |
| 2 | pass | 100 | 46 | 22.2 | 3 | 3 | [run](https://argusic.com/run/76258f98-13f3-40fb-8067-6dec1a13d8d0) |

## What was observed on a clean machine

Attempt 2:

- 4 min: `No Go toolchain in container`
- 6 min: `mkdir /var/run/wireguard: permission denied (rootless)`
- 22 min: `nylon status failed with connection refused against running daemon`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
