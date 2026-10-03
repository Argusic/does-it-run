# react-ace

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/securingsincity/react-ace, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/react-ace

## Pinned environment

- Project commit: `334f49e2681ed5c2a84847b739d821d4b8df9534`
- Test commit: `334f49e2681ed5c2a84847b739d821d4b8df9534`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 3.7 to 3.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2.5 | 3.7 | 2 | 2 | [run](https://argusic.com/run/90b8e29c-a6f6-4fd1-92a1-928111242457) |

## What was observed on a clean machine

Attempt 1:

- 1.5 min: `Node.js v18.19.1 is too old for tsdown/rolldown build tools which require Node ^22.18.0`
- 0.5 min: `tsdown failed at runtime: missing optional dependency 'unrun'`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
