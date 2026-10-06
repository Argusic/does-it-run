# agent-beacon

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Asymptote-Labs/agent-beacon, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/agent-beacon

## Pinned environment

- Project commit: `7e47847cf18fc9383af19e20d624bbcd6bc3bd3d`
- Test commit: `7e47847cf18fc9383af19e20d624bbcd6bc3bd3d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 9.1 to 9.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 8 | 9.1 | 3 | 3 | [run](https://argusic.com/run/6c236b5c-63f6-4f83-8161-69039bc7f15f) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Go 1.24+ not installed on system`
- 1 min: `Node.js v18 too old for browser-extension (needs >=22)`
- 1 min: `bun not installed and installer requires unzip (not available)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
