# setup-php

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/shivammathur/setup-php, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/setup-php

## Pinned environment

- Project commit: `f3d967b8bc6d6fbb17cb0e2ffd56cf304d0290ba`
- Test commit: `f3d967b8bc6d6fbb17cb0e2ffd56cf304d0290ba`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 5.9 to 5.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 2 | 5.9 | 1 | 1 | [run](https://argusic.com/run/3d4e53cb-f8e6-4bf3-a537-700c81eb1028) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `Array.prototype.toSorted() not available in Node 18 - ES2024 method`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
