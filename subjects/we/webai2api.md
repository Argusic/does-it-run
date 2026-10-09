# WebAI2API

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/foxhui/WebAI2API, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/webai2api

## Pinned environment

- Project commit: `beac6c979d81aea7d84a1d7b2a7e7ba686237cfb`
- Test commit: `beac6c979d81aea7d84a1d7b2a7e7ba686237cfb`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 6.7 to 6.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 6.25 | 6.7 | 3 | 3 | [run](https://argusic.com/run/93cf51bd-90d2-46d0-afa7-80cdf0227939) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `Node.js v18.19.1 lacks node:util styleText export required by @inquirer/prompts`
- 0.5 min: `pnpm not in PATH`
- 0.5 min: `pnpm install ignored build scripts for better-sqlite3 and sharp`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
