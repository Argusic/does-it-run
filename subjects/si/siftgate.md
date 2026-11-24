# SiftGate

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/seanbabalala/SiftGate, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/siftgate

## Pinned environment

- Project commit: `aa0b312432bcf9e731b6c955adec906c17421037`
- Test commit: `aa0b312432bcf9e731b6c955adec906c17421037`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 39.3 to 39.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8 | 39.3 | 0 | 0 | [run](https://argusic.com/run/0e005db5-28f0-4873-9a18-44b19324dbe6) |
| 2 | pass | 100 | 40 | 39.9 | 2 | 2 | [run](https://argusic.com/run/565a06d3-e602-4ea9-9f7f-ddaf6d34fcb0) |

## What was observed on a clean machine

Attempt 2:

- 3 min: `System Node.js v18.19.1 does not meet project requirement >=22.13.0 <23`
- 1 min: `dashboard.auth_required defaults to true with no password configured, causing startup failure`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
