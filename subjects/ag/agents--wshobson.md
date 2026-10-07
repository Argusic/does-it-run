# agents

**Verdict: runs.** Argusic Score 98.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/wshobson/agents, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/run/876142a8-feb6-4768-bd6d-e260d708114c

## Pinned environment

- Project commit: `4236bb91f8395b0435f1d8b8baf9e8e4c69a8620`
- Test commit: `4236bb91f8395b0435f1d8b8baf9e8e4c69a8620`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 3; wall time 7.9 to 19.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5.2 | 7.9 | 5 | 5 | [run](https://argusic.com/run/876142a8-feb6-4768-bd6d-e260d708114c) |
| 2 | pass | 96 | 25 | 19.7 | 5 | 4 | [run](https://argusic.com/run/e8589c66-fdf9-4696-90b3-25a581c5e874) |
| 3 | pass | 100 | 2 | 11.4 | 3 | 3 | [run](https://argusic.com/run/399d0578-e7c2-4a0b-97b5-2cb7a6c32c72) |

## What was observed on a clean machine

Attempt 1:

- 0.6 min: `uv not installed in container`
- 1 min: `pytest not installed (missing --extra dev)`
- 1 min: `ty type check failed on optional claude_agent_sdk import`
- 2 min: `npx skills fails with Node 18 (requires >=22: SyntaxError on node:util styleText)`

Attempt 2:

- 2 min: `uv not installed`
- 1 min: `claude_agent_sdk not installed, make lint fails on ty checks`
- `npx skills smoke test fails: Node v18.19.1 but skills@1.5.26 requires >=22.20.0`

Attempt 3:

- 1 min: `uv not installed`
- 1 min: `npx skills requires Node.js >=22, container has v18.19.1`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
