# OpenBot

**Verdict: could not verify.** Argusic Score 77.1 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/CopilotKit/OpenBot, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/openbot

## Pinned environment

- Project commit: `3c73cf00efba46122dfd0447485e2b61f1d6a2cd`
- Test commit: `3c73cf00efba46122dfd0447485e2b61f1d6a2cd`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 2; wall time 48.9 to 93.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | n/a | 93.2 | 0 | 0 | [run](https://argusic.com/run/b1100af3-7b7a-40c9-a7b2-c8608d9c0969) |
| 2 | fail | 77.14 | 6 | 48.9 | 7 | 6 | [run](https://argusic.com/run/38f37d69-8f60-4ac9-b85f-28e8a15c79c8) |

## What was observed on a clean machine

Attempt 2:

- 3 min: `bun not installed`
- 1 min: `agent-computer dependencies missing (playwright)`
- 1 min: `agent-langgraph dependencies missing`
- 2 min: `agent-mastra dependencies missing`
- `Docker not available (compose tests fail)`
- `PostgreSQL not available (14 integration test files fail)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
