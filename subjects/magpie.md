# magpie

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/yetone/magpie, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/magpie

## Pinned environment

- Project commit: `22358d5d6eee8b1126d3c3c0c29506685a0c89ca`
- Test commit: `22358d5d6eee8b1126d3c3c0c29506685a0c89ca`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 8.2 to 8.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8 | 8.2 | 1 | 1 | [run](https://argusic.com/run/54b0a246-2004-416f-b756-008aae545637) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Go compiler (golang) not installed in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
