# deepsec

**Verdict: runs.** Argusic Score 95 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/vercel-labs/deepsec, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/deepsec

## Pinned environment

- Project commit: `ce646748b6b2d7b088107ac29944c4129c49f11d`
- Test commit: `ce646748b6b2d7b088107ac29944c4129c49f11d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 20 to 20 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 95 | 2.5 | 20 | 4 | 3 | [run](https://argusic.com/run/9d14343f-c7f1-4140-998a-1d9200924a82) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Node v18 provided but project requires >=22`
- 0.5 min: `pnpm not found in PATH`
- 0.5 min: `Rollup native binary missing: install used --no-optional flag`
- 0.5 min: `packages/website build OOM-killed (1.9 GB RAM)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
