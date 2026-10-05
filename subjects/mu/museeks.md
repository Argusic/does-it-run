# museeks

**Verdict: could not verify.** Argusic Score 50 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/martpie/museeks, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/museeks

## Pinned environment

- Project commit: `7163f6019a3184043c06352caeec0ed1bf6ccff5`
- Test commit: `7163f6019a3184043c06352caeec0ed1bf6ccff5`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 2; wall time 54.9 to 87 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | n/a | 87 | 0 | 0 | [run](https://argusic.com/run/328dfe82-4574-49d3-b60c-aba7a0e76ba0) |
| 2 | fail | 50 | 54 | 54.9 | 7 | 7 | [run](https://argusic.com/run/1be5ff7a-b394-477c-b94c-d9a9f1391d7f) |

## What was observed on a clean machine

Attempt 2:

- 5 min: `Node.js 18.x installed, project requires >=22`
- 8 min: `Vite+ vp CLI not available and npm-installed version had native binding issues`
- 2 min: `pnpm-workspace.yaml had strictPeerDependencies:true causing install failure after vp migrate`
- 15 min: `System libraries for Tauri/webkit2gtk not installed (no root access)`
- 10 min: `Rust backend (cargo build) ran out of disk space (7.8GB total) after compiling 638 crate dependencies`
- 3 min: `E2E browser tests failed: Playwright chromium not installed`
- `E2E tests (7 tests across 3 files) timeout/fail without working Tauri backend`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
