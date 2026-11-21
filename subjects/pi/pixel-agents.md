# pixel-agents

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/pixel-agents-hq/pixel-agents, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/pixel-agents

## Pinned environment

- Project commit: `4dd14d612fd37d89ffbbc977959f572395c4eec8`
- Test commit: `4dd14d612fd37d89ffbbc977959f572395c4eec8`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 5 to 6.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 6.7 | 1 | 1 | [run](https://argusic.com/run/46e7da24-e35b-40a2-9f32-5b5f43f1828a) |
| 2 | pass | 100 | 4 | 5 | 2 | 2 | [run](https://argusic.com/run/ae0281a5-0675-4936-827a-188d9ff64719) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Node.js version 18.19.1 (required >=20, recommended 22) caused npm install warnings and rolldown native binding failures`

Attempt 2:

- 1 min: `ESLint 10.8.0 crashed on Node 18: util.styleText is not a function`
- 1 min: `Vite 8 (rolldown) fails on Node 18: styleText not available in node:util`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
