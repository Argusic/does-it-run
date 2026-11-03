# dspy-go

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/XiaoConstantine/dspy-go, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/dspy-go

## Pinned environment

- Project commit: `f2b058390e618dbd2fe58964a2eb5dea565bc86e`
- Test commit: `f2b058390e618dbd2fe58964a2eb5dea565bc86e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 9.3 to 9.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 9.3 | 1 | 1 | [run](https://argusic.com/run/d33f757d-32e7-41aa-b12a-6ccdb19bf77c) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go (golang) compiler not installed in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
