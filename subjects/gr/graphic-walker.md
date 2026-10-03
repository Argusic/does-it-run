# graphic-walker

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Kanaries/graphic-walker, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/graphic-walker

## Pinned environment

- Project commit: `869f5af40fbdf7d1e4266b3df62d9dd6d8b5f728`
- Test commit: `869f5af40fbdf7d1e4266b3df62d9dd6d8b5f728`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 12.6 to 12.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 14 | 12.6 | 3 | 3 | [run](https://argusic.com/run/6cb8ae30-0685-43d7-8c00-9b79471d2153) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Node engine constraint >=20.0.0 unmet by container's Node 18.19.1`
- 1 min: `yarn not pre-installed in container`
- `duckdb-wasm-computation build crashes with OOM/core dump (exit 134)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
