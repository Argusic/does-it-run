# coai

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/coaidev/coai, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/coai

## Pinned environment

- Project commit: `3048a493eedcfe75de4d59afd5139847ad3195ed`
- Test commit: `3048a493eedcfe75de4d59afd5139847ad3195ed`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 17.7 to 17.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 17 | 17.7 | 5 | 5 | [run](https://argusic.com/run/87b2694e-f197-401e-9dea-c0ef8c868207) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go not installed in container`
- 1 min: `pnpm not installed`
- 4 min: `pnpm ignored build scripts for @swc/core and esbuild`
- 1 min: `SQLite migration error (duplicate column name)`
- 5 min: `Redis not available (server requires Redis)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
