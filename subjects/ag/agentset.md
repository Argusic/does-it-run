# agentset

**Verdict: runs with mocks.** Argusic Score 56 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/agentset-ai/agentset, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/agentset

## Pinned environment

- Project commit: `03283cc6383b96facbec53190ed352079b641789`
- Test commit: `03283cc6383b96facbec53190ed352079b641789`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 31.9 to 41.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 31.9 | 0 | 0 | [run](https://argusic.com/run/30eaada4-2a9c-4a88-b4e7-cc514b757240) |
| 2 | pass with mocks | 92 | 25 | 41.7 | 5 | 5 | [run](https://argusic.com/run/0891f4ce-3494-4a09-bce4-0f6d666394fd) |

## What was observed on a clean machine

Attempt 2:

- 3 min: `bun not installed and unzip not available`
- 5 min: `bun preinstall script failed: Prisma requires Node >=22.12 but system has Node 18.19.1`
- 4 min: `prisma generate failed: missing DIRECT_URL env var; schema file needed explicit path`
- 3 min: `prisma enums generated empty because --schema pointed to single file instead of directory`
- 10 min: `zod/v4 import { z } resolves as undefined in vitest/vite due to chained re-export of namespace import`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
