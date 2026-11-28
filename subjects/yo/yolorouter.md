# yolorouter

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/yolorouter/yolorouter, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/yolorouter

## Pinned environment

- Project commit: `f7cd3c3e7fc212119925e5929a122b6a6fb68e9d`
- Test commit: `f7cd3c3e7fc212119925e5929a122b6a6fb68e9d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 7 to 7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 11 | 7 | 2 | 2 | [run](https://argusic.com/run/2c006915-0dea-4a02-a710-c2d1d822392d) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go 1.25.7+ required but not installed; OS package (golang-go 1.22) too old`
- 2 min: `Test TestSlidingWriteDeadlineCutsSlowClient failed: TCP send buffer on loopback (default 1MB wmem) absorbed all 100x64KB writes within 150ms window, never causing Write to block`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
