# openfuse

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/CopilotKit/openfuse, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/openfuse

## Pinned environment

- Project commit: `7771e2db03a4b25d8bc8ee32f7a5c0dddafe3bfc`
- Test commit: `7771e2db03a4b25d8bc8ee32f7a5c0dddafe3bfc`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 7.9 to 7.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 3.5 | 7.9 | 3 | 3 | [run](https://argusic.com/run/e64c7f85-a8b1-4315-a7b3-09ede93b76c4) |

## What was observed on a clean machine

Attempt 1:

- 0.25 min: `Node.js v18.19.1 is below the required >=22`
- 0.1 min: `pnpm not installed`
- 0.1 min: `CPK_INTELLIGENCE_API_KEY is required at startup`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
