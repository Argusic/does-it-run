# mcp-language-server

**Verdict: runs.** Argusic Score 93.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/isaacphi/mcp-language-server, licensed BSD-3-Clause, written in Go.

Evidence and recordings: https://argusic.com/subject/mcp-language-server

## Pinned environment

- Project commit: `e4395849a52e18555361abab60a060802c06bf50`
- Test commit: `e4395849a52e18555361abab60a060802c06bf50`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 61.8 to 61.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 93.33 | 67 | 61.8 | 9 | 6 | [run](https://argusic.com/run/b653c109-b342-488e-86a3-7a5668104b8a) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Go not installed`
- 5 min: `Watcher tests had race condition: events channel not drained on ResetEvents, causing stale signals`
- 2 min: `Go hover snapshots mismatched (gopls v0.23.0 outputs different struct size format)`
- 2 min: `Python hover snapshots mismatched (pyright 1.1.414 outputs different hover format)`
- 2 min: `Rust integration test snapshots mismatched (rust-analyzer 1.99.0)`
- 1 min: `TypeScript tests failed: typescript-language-server requires TypeScript installed in workspace`
- `Rust diagnostics FileDependency test timing-dependent failure in constrained container`
- `Rust references helper_function test timing-dependent failure under concurrency`
- `clangd integration tests fail (clangd not in container)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
