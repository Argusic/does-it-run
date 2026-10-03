# frp

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/fatedier/frp, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/frp

## Pinned environment

- Project commit: `d20a232996007dfe6ab425abc0a39a3ae9a0889b`
- Test commit: `d20a232996007dfe6ab425abc0a39a3ae9a0889b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 6 to 6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 6 | 1 | 1 | [run](https://argusic.com/run/d1c3f059-6741-4ff2-a21d-d077370155fb) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go 1.25.0 required but not installed in environment`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
