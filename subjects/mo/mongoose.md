# mongoose

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/nestjs/mongoose, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/mongoose

## Pinned environment

- Project commit: `2d7ad82e63a9f1a40d6f7ae0abc89045d8df2f73`
- Test commit: `2d7ad82e63a9f1a40d6f7ae0abc89045d8df2f73`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 7.4 to 7.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 7 | 7.4 | 3 | 3 | [run](https://argusic.com/run/173ff58f-5cd1-4b23-a3c0-1aa8f2e643f8) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node.js v18.19.1 missing styleText export from node:util required by vitest 5`
- 3 min: `No MongoDB server available for integration tests`
- 1 min: `Lazy connection test timed out`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
