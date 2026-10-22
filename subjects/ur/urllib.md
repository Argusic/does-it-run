# urllib

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/node-modules/urllib, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/urllib

## Pinned environment

- Project commit: `9d183f2824cb7f8511f97ddbb8d59dc92fba4137`
- Test commit: `9d183f2824cb7f8511f97ddbb8d59dc92fba4137`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 4.3 to 4.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 4.2 | 4.3 | 2 | 2 | [run](https://argusic.com/run/1930e8c8-62ad-4633-a5e7-355c6fd0bd36) |

## What was observed on a clean machine

Attempt 1:

- 3.5 min: `System Node.js v18.19.1 is too old for vite-plus prepare script (needs styleText from node:util, available in v22+)`
- 0.5 min: `Formatting check failed on package.json`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
