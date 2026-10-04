# Claw3D

**Verdict: runs.** Argusic Score 90 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/iamlukethedev/Claw3D, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/claw3d

## Pinned environment

- Project commit: `0565b7892909eca7bbc8f2d9b0fad171dd75ad7c`
- Test commit: `0565b7892909eca7bbc8f2d9b0fad171dd75ad7c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 75.2 to 87 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | n/a | 87 | 0 | 0 | [run](https://argusic.com/run/c97e3d87-89f4-4b76-8bf2-4bbbd6ea7809) |
| 2 | pass | 90 | 5 | 75.2 | 2 | 1 | [run](https://argusic.com/run/c7a995d3-acbb-4420-9e00-803703456c9c) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `Node.js v18.19.1 was the default but the project requires >=20.`
- `5 pre-existing vitest test failures across 4 test files (agentFleetHydration, useGatewayConnection, useAgentSettingsMutationController, agentChatPanel-controls, taskBoardView)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
