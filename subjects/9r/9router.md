# 9router

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/decolua/9router, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/9router

## Pinned environment

- Project commit: `39e36d3d0c849e0e01dfeacddf111edf892448fc`
- Test commit: `39e36d3d0c849e0e01dfeacddf111edf892448fc`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 42 to 42 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8.2 | 42 | 3 | 3 | [run](https://argusic.com/run/6c9de159-ad3b-4e6f-bf1e-43978c798ae8) |

## What was observed on a clean machine

Attempt 1:

- 1.5 min: `Node.js v18.19.1 too old for Next.js 16 (requires >=20.9.0)`
- 0.5 min: `npm install in tests/ failed with Cannot read properties of null (reading edgesOut)`
- 1 min: `vitest 4.x native binding error for rolldown (missing @rolldown/binding-wasm32-wasi)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
