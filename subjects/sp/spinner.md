# spinner

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/briandowns/spinner, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/spinner

## Pinned environment

- Project commit: `b8e40ed483c4e21877add43fd71db416c0e154e8`
- Test commit: `b8e40ed483c4e21877add43fd71db416c0e154e8`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 5.6 to 8.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 5.6 | 0 | 0 | [run](https://argusic.com/run/c15dc077-e047-4144-bc53-76d4fd691f76) |
| 2 | pass | 100 | 4 | 8.2 | 2 | 2 | [run](https://argusic.com/run/1fc477ec-acfa-43b2-b65e-47b3d129853e) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `No Go+ (Go programming language) compiler binary found on system`
- 2 min: `Standard library packages missing from Go+ compiler installation (errors, fmt, bytes, etc.)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
