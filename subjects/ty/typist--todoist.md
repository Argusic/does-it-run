# typist

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/todoist/typist, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/run/cd13cbd5-b360-4733-bd93-4eddbd31ae9d

## Pinned environment

- Project commit: `7e0234ee3a9a74767d9176ccc5ece11fcee87a0b`
- Test commit: `7e0234ee3a9a74767d9176ccc5ece11fcee87a0b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 2.4 to 2.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.8 | 2.4 | 2 | 2 | [run](https://argusic.com/run/cd13cbd5-b360-4733-bd93-4eddbd31ae9d) |

## What was observed on a clean machine

Attempt 1:

- 0.3 min: `Host Node.js v18.19.1 did not satisfy the project's devEngines requirement (>= 24.15.0)`
- 0.1 min: `Initial npm install failed because devEngines required Node >= 24.15.0 but 24.13.0 was in use`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
