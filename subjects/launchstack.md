# LaunchStack

**Verdict: runs.** Argusic Score 90 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Deodat-Lawson/LaunchStack, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/launchstack

## Pinned environment

- Project commit: `a2fb47de0aae64d3a904bec3c319b46527caae0a`
- Test commit: `a2fb47de0aae64d3a904bec3c319b46527caae0a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 26.4 to 33.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 0.5 | 26.4 | 3 | 3 | [run](https://argusic.com/run/216cced6-98f7-4566-bcab-0a813a6ee9fd) |
| 2 | pass | 100 | 45 | 33.2 | 5 | 5 | [run](https://argusic.com/run/a75994bb-3b3c-493a-a0f0-114b97c17eca) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Node.js v18.19.1 present but project requires >=20`
- 0.5 min: `pnpm 10.15.1 not found at PATH`
- 0.5 min: `Landing page build failed on stale .next/cache from previous build`

Attempt 2:

- 2 min: `Node v18.19.1 below required ≥20`
- 1 min: `pnpm not installed`
- 1 min: `rollup-linux-x64-gnu native optional dependency missing`
- 8 min: `PostgreSQL not available (README expects Docker Compose)`
- 1 min: `Jest setup did not load .env so integration tests skipped`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
