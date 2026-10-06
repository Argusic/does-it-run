# agent-ui

**Verdict: could not verify.** Argusic Score 80 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/agno-agi/agent-ui, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/agent-ui

## Pinned environment

- Project commit: `6dad9593fca6756e1813e4f4b3b2620be6377691`
- Test commit: `6dad9593fca6756e1813e4f4b3b2620be6377691`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 2; wall time 3.4 to 10.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 2 | 3.4 | 2 | 2 | [run](https://argusic.com/run/51a0bbff-e3d5-4cd1-9b7f-aa725da06167) |
| 2 | fail | 80 | 2 | 10.7 | 2 | 2 | [run](https://argusic.com/run/d3e45241-b7be-4ede-85e1-68d7520d7ae3) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `pnpm not installed`
- 0.5 min: `pnpm install blocked by sharp build script policy`

Attempt 2:

- 2 min: `pnpm not found in system`
- 1 min: `pnpm install blocked by build policy for sharp`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
