# setup-php

**Verdict: runs.** Argusic Score 91 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/shivammathur/setup-php, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/setup-php

## Pinned environment

- Project commit: `f3d967b8bc6d6fbb17cb0e2ffd56cf304d0290ba`
- Test commit: `f3d967b8bc6d6fbb17cb0e2ffd56cf304d0290ba`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 5.9 to 13.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 2 | 5.9 | 1 | 1 | [run](https://argusic.com/run/3d4e53cb-f8e6-4bf3-a537-700c81eb1028) |
| 2 | pass | 90 | 6 | 13.9 | 2 | 1 | [run](https://argusic.com/run/adcea05a-423d-4803-ba94-5f1489d78657) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `Array.prototype.toSorted() not available in Node 18 - ES2024 method`

Attempt 2:

- 8 min: `npm test under container Node 18.19.1: 11 failures with TypeError: releases.toSorted is not a function (src/tools.ts:252,221; repo requires Node>=20, CI pins 24.x)`
- 14 min: `node dist/index.js: action starts but cannot install PHP in this container - src/scripts/linux.sh:288 fails 'sudo: command not found' and apt-get install sudo fails (no root), so run loops until 300s timeout (exit 124)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
