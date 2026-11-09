# react-lifecycle-methods-diagram

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/wojtekmaj/react-lifecycle-methods-diagram, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/react-lifecycle-methods-diagram

## Pinned environment

- Project commit: `754a487fbc8cd3190e452c3f49a2a317631249fe`
- Test commit: `754a487fbc8cd3190e452c3f49a2a317631249fe`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 1.7 to 10 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 10 | 2 | 2 | [run](https://argusic.com/run/99a62b5f-524f-4ecb-8db5-03cc128af06f) |
| 2 | pass | 100 | 15 | 1.7 | 2 | 2 | [run](https://argusic.com/run/ae0a2b24-2e5a-4541-aa3f-bc6952fbe0c5) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node.js v18.19.1 too old for Vite 8 (requires node 20.19+).`
- 3.5 min: `System yarn 1.22.22 blocked by packageManager field requiring yarn@4.17.1; corepack not available on node v18.`

Attempt 2:

- 3 min: `Node.js 18.19.1 too old for Vite 8 (needs 20.19+ or 22.12+)`
- 2 min: `Yarn not installed on system`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
