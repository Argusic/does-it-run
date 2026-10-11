# copilot-api

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/caozhiyuan/copilot-api, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/copilot-api

## Pinned environment

- Project commit: `ab4e0360cb9c4f5c711439619af8e7d6bade1b22`
- Test commit: `ab4e0360cb9c4f5c711439619af8e7d6bade1b22`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 17.1 to 17.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 35 | 17.1 | 3 | 3 | [run](https://argusic.com/run/4ad48dc4-cb26-4688-b258-cea4d8957d1c) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Bun not pre-installed; Node.js v18 too old for tsdown build (needs node:util.styleText)`
- 5 min: `Server blocks on interactive provider selection prompt when no providers are configured`
- `No real third-party API keys available to test against live upstreams`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
