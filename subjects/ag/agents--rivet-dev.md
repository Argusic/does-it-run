# agents

**Verdict: runs.** Argusic Score 93.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/rivet-dev/agents, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/run/196d3a61-80b5-446c-ad66-eb86c7424755

## Pinned environment

- Project commit: `07fa4fb44a78f782f0ef64e2c273f67b56b29921`
- Test commit: `07fa4fb44a78f782f0ef64e2c273f67b56b29921`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 39.4 to 39.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 93.33 | 38 | 39.4 | 3 | 2 | [run](https://argusic.com/run/196d3a61-80b5-446c-ad66-eb86c7424755) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Node v18.19.1 in container, project requires >=22.19.0`
- 1 min: `pnpm not available after switching Node versions`
- `3 pre-existing test flakes: caller-disconnect(2) and durable-watch(1) , timing-sensitive race conditions unrelated to install`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
