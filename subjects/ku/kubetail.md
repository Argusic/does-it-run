# kubetail

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/kubetail-org/kubetail, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/kubetail

## Pinned environment

- Project commit: `ba74e7bfa38aac317c62f5196ec9b65f386b4613`
- Test commit: `ba74e7bfa38aac317c62f5196ec9b65f386b4613`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 16.5 to 16.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 15 | 16.5 | 5 | 5 | [run](https://argusic.com/run/c2a101e6-9fc8-45c1-8de1-95d290d997b3) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go not found in container`
- 1 min: `pnpm not found in container`
- 3 min: `Node 18.19.1 too old for rolldown (requires >=22.12.0)`
- 1 min: `Leftover node_modules_old directory caused vitest to import stale jest-dom and zod tests, producing 12 failed test files`
- `No Rust toolchain in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
