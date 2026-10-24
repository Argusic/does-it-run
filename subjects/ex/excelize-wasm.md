# excelize-wasm

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/xuri/excelize-wasm, licensed BSD-3-Clause, written in Go.

Evidence and recordings: https://argusic.com/subject/excelize-wasm

## Pinned environment

- Project commit: `a11a6f1ba5d833f10d887cb3217433a1c2b3da40`
- Test commit: `a11a6f1ba5d833f10d887cb3217433a1c2b3da40`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 12.7 to 12.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 10 | 12.7 | 2 | 2 | [run](https://argusic.com/run/9e465fd3-aaab-482e-83d2-313691399672) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `rollup build failed: crypto is not defined in serialize-javascript (dependency of @rollup/plugin-terser)`
- 2 min: `excelize.wasm.gz missing from source repo; requires Go compilation`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
