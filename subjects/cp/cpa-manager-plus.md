# CPA-Manager-Plus

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/seakee/CPA-Manager-Plus, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/cpa-manager-plus

## Pinned environment

- Project commit: `eea422fd6a19ddb90f117b79b80d1f785a3b6a83`
- Test commit: `eea422fd6a19ddb90f117b79b80d1f785a3b6a83`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 11.6 to 11.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 11.6 | 1 | 1 | [run](https://argusic.com/run/dcbc2a63-92a0-47d0-94e2-9330e5cede4a) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `System Node.js v18.19.1 is too old (project requires ^20.19.0 or >=22.12.0)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
