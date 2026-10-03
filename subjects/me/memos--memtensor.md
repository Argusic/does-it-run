# MemOS

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/MemTensor/MemOS, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/run/a92789ba-3e9a-4bac-9225-2618fcffa7e5

## Pinned environment

- Project commit: `a7367d07e55db61099f7b4e2c1108bc5831a24f3`
- Test commit: `a7367d07e55db61099f7b4e2c1108bc5831a24f3`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 5.1 to 5.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 8 | 5.1 | 2 | 2 | [run](https://argusic.com/run/a92789ba-3e9a-4bac-9225-2618fcffa7e5) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `API server (uvicorn) cannot start , init_server() eagerly connects to Qdrant on localhost:6333 which isn't running`
- `memos export_openapi fails , same eager init_server() call at module import`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
