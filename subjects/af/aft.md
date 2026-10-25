# aft

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/cortexkit/aft, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/aft

## Pinned environment

- Project commit: `17f2c807c9f5df1b55e40b4efce3bd54e3262ecc`
- Test commit: `17f2c807c9f5df1b55e40b4efce3bd54e3262ecc`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 54.5 to 54.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 54.2 | 54.5 | 6 | 6 | [run](https://argusic.com/run/57627b41-fe19-4fc7-8cac-2ac37eb1b9be) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `Missing rustc and cargo toolchain`
- 0.5 min: `Missing bun runtime`
- 4 min: `Missing unzip binary - 5 TypeScript tests failed`
- 2 min: `Rust lib tests: InsecureParentDirectory error in 24 gh_shim/subc tests`
- 8 min: `Rust lib tests: 3 agent_child_env hook tests failed (duplicate Co-authored-by trailers)`
- 1 min: `Pi plugin: read vision capability test used legacy gh_read config key`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
