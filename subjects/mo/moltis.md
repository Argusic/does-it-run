# moltis

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/moltis-org/moltis, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/moltis

## Pinned environment

- Project commit: `9c7ea0700a873b77733733a977484f86a2808d4d`
- Test commit: `9c7ea0700a873b77733733a977484f86a2808d4d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 21.1 to 48.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 19 | 21.1 | 3 | 3 | [run](https://argusic.com/run/2d7e1379-c5a6-4383-b9e3-7c3c26af568a) |
| 2 | pass with mocks | 92 | 30 | 48.4 | 4 | 4 | [run](https://argusic.com/run/9c4d646d-bec7-4327-8c20-468facadb3ce) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Rust toolchain not installed`
- 1 min: `Node.js v18 too old for Vite 8 (needs ^20.19.0 || >=22.12.0)`

Attempt 2:

- 1 min: `Rust toolchain not installed (no rustc/cargo)`
- `3 test failures in moltis-httpd: ssh_keygen not found on system`
- `2 test failures in moltis-tools: WASM sandbox not compiled + flaky docker fallback test`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
