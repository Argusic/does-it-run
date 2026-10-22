# summon

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/cyberark/summon, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/summon

## Pinned environment

- Project commit: `d42f0517dd7ef31e6cbbadb6e1963394d6aab90b`
- Test commit: `d42f0517dd7ef31e6cbbadb6e1963394d6aab90b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 4.8 to 4.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 4.8 | 2 | 2 | [run](https://argusic.com/run/964beb47-23cf-4d54-b5e2-1e76b284a23b) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `go: not found in container (no Go toolchain, no Docker for the scripted test path)`
- 1 min: `mock Conjur server exited after its launching shell ended (connection refused)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
