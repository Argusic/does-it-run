# jev-job-search

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/qbeka/jev-job-search, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/jev-job-search

## Pinned environment

- Project commit: `6311a3997e8bda49a0164106df5ba7b8e885301c`
- Test commit: `6311a3997e8bda49a0164106df5ba7b8e885301c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 1.6 to 1.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.5 | 1.6 | 2 | 2 | [run](https://argusic.com/run/61642bbd-9a8b-471f-b137-e2919483e3ad) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `Node.js v18.19.1 installed but project requires >=22`
- `Google Chrome not found , this is a macOS-only tool that needs Chrome for browser tests`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
