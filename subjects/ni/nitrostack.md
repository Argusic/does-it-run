# nitrostack

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/nitrocloudofficial/nitrostack, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/nitrostack

## Pinned environment

- Project commit: `4c1a1c472d8e2c6001e700d34f128009b9284b4e`
- Test commit: `4c1a1c472d8e2c6001e700d34f128009b9284b4e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 53.1 to 75.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 53.1 | 0 | 0 | [run](https://argusic.com/run/c47e198e-2966-4c0b-a4fb-f402028beec7) |
| 2 | pass | 100 | 1 | 75.1 | 2 | 2 | [run](https://argusic.com/run/3b14b158-7f07-4592-a146-77ba0a38959c) |

## What was observed on a clean machine

Attempt 2:

- 15 min: `@modelcontextprotocol/server v2 SDK uses bare 'crypto.randomUUID()' which is not available as a global in Node.js 18 module context (only -e eval)`
- 20 min: `Widget bridge tests fail in full suite due to jsdom having window.parent === window as a read-only computed property (Object.defineProperty cannot override it)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
