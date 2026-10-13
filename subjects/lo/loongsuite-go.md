# loongsuite-go

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/alibaba/loongsuite-go, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/loongsuite-go

## Pinned environment

- Project commit: `cac400935add57d8219122ba32857b8f55ac6eb1`
- Test commit: `cac400935add57d8219122ba32857b8f55ac6eb1`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 32.6 to 32.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 32.6 | 2 | 2 | [run](https://argusic.com/run/2f9d13bc-f6a6-41b7-ad15-ce665ab5b912) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go 1.25+ not installed in container`
- 1 min: `non-constant format string in vet check (Go 1.25 strictness)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
