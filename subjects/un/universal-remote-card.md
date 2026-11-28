# universal-remote-card

**Verdict: could not verify.** Argusic Score 80 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Nerwyn/universal-remote-card, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/universal-remote-card

## Pinned environment

- Project commit: `9aad7dc0fb55bf932f81fd306e5e0076ec075df0`
- Test commit: `9aad7dc0fb55bf932f81fd306e5e0076ec075df0`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 2; wall time 1.3 to 2.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 0.5 | 1.3 | 1 | 1 | [run](https://argusic.com/run/2cdf7bf9-28d1-46f5-8d31-1af35396ec31) |
| 2 | fail | 80 | 5 | 2.1 | 1 | 1 | [run](https://argusic.com/run/71f2a579-af77-42a5-b94e-ea7ad49e76fb) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Rspack requires Node.js 20.19+ but container had Node.js 18.19.1`

Attempt 2:

- 2 min: `Rspack 2.0.1 requires Node.js 20.19+ but container has Node 18.19.1`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
