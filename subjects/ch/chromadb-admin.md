# chromadb-admin

**Verdict: not yet verified.** Argusic Score 80 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/flanker/chromadb-admin, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/chromadb-admin

## Pinned environment

- Project commit: `efe867c86c78683d90b0eb74b88b351fc08f0b5f`
- Test commit: `efe867c86c78683d90b0eb74b88b351fc08f0b5f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 1; wall time 11.8 to 11.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 7 | 11.8 | 1 | 1 | [run](https://argusic.com/run/0d2a16fb-2c9a-4970-94cd-90b2775c914d) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `API collections route threw error on unhandled exception, crashing the server instead of returning a 500 response`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
