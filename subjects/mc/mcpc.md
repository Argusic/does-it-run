# mcpc

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/apify/mcpc, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/mcpc

## Pinned environment

- Project commit: `a8c34fc1af1f89626218712d940b673206a69ed6`
- Test commit: `a8c34fc1af1f89626218712d940b673206a69ed6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 5.9 to 18.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1 | 5.9 | 0 | 0 | [run](https://argusic.com/run/b21a1f33-09c2-461a-b32d-bec6a602a830) |
| 2 | pass | 100 | 1 | 18.4 | 2 | 2 | [run](https://argusic.com/run/73b06582-2b29-49cb-b3f3-8a51387d56df) |

## What was observed on a clean machine

Attempt 2:

- 0.5 min: `Node.js v18 was installed but project requires >=22.12`
- 0.1 min: `pnpm was not installed`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
