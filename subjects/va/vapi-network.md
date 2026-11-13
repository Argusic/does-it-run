# vapi-network

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/vAPI-Network/vapi-network, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/vapi-network

## Pinned environment

- Project commit: `1cafa80f0f94a3459f4c7a66d8617f2fa40becf1`
- Test commit: `1cafa80f0f94a3459f4c7a66d8617f2fa40becf1`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 7.5 to 12.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1 | 12.1 | 1 | 1 | [run](https://argusic.com/run/e30ee3c1-4881-4f84-bef1-75ebee2b89ef) |
| 2 | pass with mocks | 92 | 10 | 7.5 | 1 | 1 | [run](https://argusic.com/run/94989f41-80dd-4acc-9915-400210ba529d) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Test timeout in src/swarm.test.ts at 5s default (flaky under parallel load)`

Attempt 2:

- 3 min: `Node.js 22 required but v18.19.1 present; pnpm 10.27.0 required but 9.2.0 present`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
