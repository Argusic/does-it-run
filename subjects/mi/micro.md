# micro

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/micro-editor/micro, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/micro

## Pinned environment

- Project commit: `7484d5f5fa95d3dfb025a01b09f31a1b0e7f9b1b`
- Test commit: `7484d5f5fa95d3dfb025a01b09f31a1b0e7f9b1b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 2.3 to 2.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 2.7 | 0 | 0 | [run](https://argusic.com/run/6ba5a315-be62-4bb3-9998-5529e3fced27) |
| 2 | pass | 100 | 7 | 2.3 | 1 | 1 | [run](https://argusic.com/run/ae5c03a8-88d5-4ef0-8b42-f5f3180745f0) |

## What was observed on a clean machine

Attempt 2:

- 5 min: `Go toolchain missing ('go: not found')`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
