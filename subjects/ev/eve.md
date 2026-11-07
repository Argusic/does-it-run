# eve

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/vercel/eve, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/eve

## Pinned environment

- Project commit: `a7b0fb2bf24d57e6bb3613d557c0af53a171d558`
- Test commit: `a7b0fb2bf24d57e6bb3613d557c0af53a171d558`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 9.2 to 13.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 13 | 13.8 | 0 | 0 | [run](https://argusic.com/run/061abccb-239d-41a9-98a3-e43f57db9ab9) |
| 2 | pass | 100 | 2 | 9.2 | 1 | 1 | [run](https://argusic.com/run/4dd524ea-0319-4537-aba1-d5982ce5ef77) |

## What was observed on a clean machine

Attempt 2:

- `pnpm typecheck workspace-wide exited 137 (OOM) , container ran out of memory with 51 concurrent tsc processes`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
