# typeorm

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/nestjs/typeorm, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/run/8c9a40fc-6053-46e4-927a-b74762ca0287

## Pinned environment

- Project commit: `a268eebf05d10fdc245286e60815aca2bacfab7a`
- Test commit: `a268eebf05d10fdc245286e60815aca2bacfab7a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 9.1 to 9.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8 | 9.1 | 2 | 2 | [run](https://argusic.com/run/8c9a40fc-6053-46e4-927a-b74762ca0287) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node.js v18.19.1 too old for vitest 5.x , rolldown requires styleText from node:util (Node >=20)`
- 4 min: `PostgreSQL 16 not installed , e2e tests require a running postgres instance accepting connections`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
