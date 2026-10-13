# webkubectl

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/1Panel-dev/webkubectl, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/webkubectl

## Pinned environment

- Project commit: `77be0d7c28ec181eba6f7b665c0bb9194e9b76a4`
- Test commit: `77be0d7c28ec181eba6f7b665c0bb9194e9b76a4`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 6.3 to 6.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 7 | 6.3 | 5 | 5 | [run](https://argusic.com/run/b561d973-27ef-47aa-bcce-7f086484782e) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go compiler not installed`
- 1 min: `kubectl not installed`
- 3 min: `Pre-built /usr/bin/gotty is upstream version without webkubectl API`
- `unshare fails in container (no --privileged)`
- `go test fails - webtty_test.go references undefined symbols`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
