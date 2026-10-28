# oh-my-cpa

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/WizisCool/oh-my-cpa, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/oh-my-cpa

## Pinned environment

- Project commit: `671dfe51c6e3d51084577f190c32dfd88ef3497e`
- Test commit: `671dfe51c6e3d51084577f190c32dfd88ef3497e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 16 to 16 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 15.75 | 16 | 4 | 4 | [run](https://argusic.com/run/3678ca32-6594-44ea-ba39-3512de2e81ea) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go 1.27.1 not in PATH; go binary absent`
- 2.5 min: `Node.js is v18.19.1, requires v22.23.2`
- 1 min: `pnpm not found`
- `2 repository-test failures in maintenance/weekly lanes (fuzz and advisory)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
