# betteroffice

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/openooxml/betteroffice, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/betteroffice

## Pinned environment

- Project commit: `1af946fc0ef64a87232a5d452a6395415169694d`
- Test commit: `1af946fc0ef64a87232a5d452a6395415169694d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 23.3 to 49.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 25 | 23.3 | 6 | 6 | [run](https://argusic.com/run/f140feb1-d3d5-44ab-a24a-3b9d32de3b88) |
| 2 | pass | 100 | 35 | 49.8 | 8 | 8 | [run](https://argusic.com/run/911f3211-5f31-4045-a73e-cb3a11d0621d) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `bun not found in container`
- 2 min: `cargo/rustc not found in container`
- 2 min: `wasm-pack not found`
- 1 min: `wasm-opt not found`
- 1 min: `fonts package not built (unmet peer dependency)`
- 1 min: `pptx WASM module not built`

Attempt 2:

- 3 min: `Rust toolchain not installed`
- 5 min: `Bun not installed; no root for apt-get`
- 3 min: `wasm-pack 0.15.0 not installed`
- 2 min: `wasm-opt not found`
- 1 min: `Response body already used errors in check-publish-targets.test.ts`
- 4 min: `Node.js 18 too old for wrangler (needs >=22)`
- 1 min: `@betteroffice/fonts not built`
- 1 min: `pptx-wasm binary not built (ppt tests failing)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
