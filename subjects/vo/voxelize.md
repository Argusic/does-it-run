# voxelize

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/voxelize/voxelize, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/voxelize

## Pinned environment

- Project commit: `b5097e45acba0b5e4c457eb7c4294a6797b2b485`
- Test commit: `b5097e45acba0b5e4c457eb7c4294a6797b2b485`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 21.1 to 26.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 26 | 26.7 | 3 | 3 | [run](https://argusic.com/run/d9e29504-dcc5-4d6c-ad8e-95c4f3a953a3) |
| 2 | pass | 100 | 20 | 21.1 | 7 | 7 | [run](https://argusic.com/run/6785cdf8-1ddb-4dbe-a2a1-26f305cf152b) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `frame-budget.test.ts: performance.now is read-only in Node 18 (11 tests failed)`
- 2 min: `vitest picked up scripts/engine-boundary/check.test.mjs as a test suite but it uses Node native test runner`
- 1 min: `geology_cost_smoke test: p95 geo chunk cost 538781us blew smoke bound in constrained environment`

Attempt 2:

- 2 min: `Rust toolchain missing (rustc, cargo not found)`
- 1 min: `pnpm not installed`
- 1 min: `wasm-pack not installed`
- 1 min: `protoc not installed`
- 3 min: `cargo-watch not installed`
- 2 min: `frame-budget.test.ts: 11 failures - Cannot assign to read only property now of Performance (Node 18 compat)`
- 1 min: `scripts/engine-boundary/check.test.mjs picked up by vitest (uses node:test, not vitest)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
