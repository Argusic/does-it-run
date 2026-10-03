# zerolang

**Verdict: runs.** Argusic Score 93.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/vercel-labs/zerolang, licensed Apache-2.0, written in C.

Evidence and recordings: https://argusic.com/subject/zerolang

## Pinned environment

- Project commit: `7e1a64d27cc37671df31c6370890bce86f5135e1`
- Test commit: `7e1a64d27cc37671df31c6370890bce86f5135e1`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 45.7 to 45.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 93.33 | 6 | 45.7 | 3 | 2 | [run](https://argusic.com/run/6c055445-551c-47a4-96bf-a39daf5b0e9c) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Node.js v18 installed but project requires >=24`
- 2 min: `pnpm not installed`
- 5 min: `Cross-target linux-musl-x64 tests require bundled musl toolchain not in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
