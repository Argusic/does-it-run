# dex

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/dcramer/dex, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/dex

## Pinned environment

- Project commit: `3f55b2a3ec9746fc56cf62037ca6a828555ce17d`
- Test commit: `3f55b2a3ec9746fc56cf62037ca6a828555ce17d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 5.3 to 5.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.23 | 5.3 | 2 | 2 | [run](https://argusic.com/run/bb165576-c656-4f0e-82e2-ed9f75e3e5ac) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `pnpm not in PATH after npm global install`
- 2 min: `Array.prototype.toSorted is not available in Node 18 (project requires Node >=24)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
