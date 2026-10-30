# kanban-md

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/antopolskiy/kanban-md, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/kanban-md

## Pinned environment

- Project commit: `6f01678748ac44027b58ca98ce62a680ec899963`
- Test commit: `6f01678748ac44027b58ca98ce62a680ec899963`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 6.4 to 6.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 6 | 6.4 | 2 | 2 | [run](https://argusic.com/run/dffcd2d5-5296-4619-a73d-6ed420c99a4d) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go not found in container`
- 3 min: `golangci-lint not found`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
