# deeporg

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/dosco/deeporg, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/deeporg

## Pinned environment

- Project commit: `bea1c714c5b8499b83461af722719c0b0cb9679a`
- Test commit: `bea1c714c5b8499b83461af722719c0b0cb9679a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 5.1 to 6.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 5.1 | 2 | 2 | [run](https://argusic.com/run/bdc12bf5-aa22-40b7-84d7-d6cbcfc43d38) |
| 2 | pass | 100 | 7 | 6.8 | 0 | 0 | [run](https://argusic.com/run/4df1c471-b158-48fc-af52-6126825f454f) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `go: not found (Go toolchain missing in container)`
- 1 min: `go build ./cmd/... failed: build output cmd already exists and is a directory`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
