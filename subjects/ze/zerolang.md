# zerolang

**Verdict: runs.** Argusic Score 96.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/vercel-labs/zerolang, licensed Apache-2.0, written in C.

Evidence and recordings: https://argusic.com/subject/zerolang

## Pinned environment

- Project commit: `7e1a64d27cc37671df31c6370890bce86f5135e1`
- Test commit: `7e1a64d27cc37671df31c6370890bce86f5135e1`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 12.2 to 45.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 93.33 | 6 | 45.7 | 3 | 2 | [run](https://argusic.com/run/6c055445-551c-47a4-96bf-a39daf5b0e9c) |
| 2 | pass | 100 | 2 | 12.2 | 3 | 3 | [run](https://argusic.com/run/6ca2798b-4135-4865-bfe8-3e13952da311) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Node.js v18 installed but project requires >=24`
- 2 min: `pnpm not installed`
- 5 min: `Cross-target linux-musl-x64 tests require bundled musl toolchain not in container`

Attempt 2:

- 0.5 min: `System Node.js v18.19.1 < required v24`
- 0.1 min: `pnpm not installed`
- `Cross-compilation to linux-musl-x64 requires musl-capable C compiler, not available`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
