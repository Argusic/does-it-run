# MikroDash

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/SecOps-7/MikroDash, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/mikrodash

## Pinned environment

- Project commit: `2269c083b8d1ae3a22c043f043b6ad9764085c84`
- Test commit: `2269c083b8d1ae3a22c043f043b6ad9764085c84`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 10 to 42.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 42 | 42.2 | 5 | 5 | [run](https://argusic.com/run/2b0487d8-eb46-4d29-aa08-2b8578e9c12e) |
| 2 | pass | 100 | 5 | 10 | 1 | 1 | [run](https://argusic.com/run/8b85bcd2-cd5f-4bde-8153-d7c2e3040081) |

## What was observed on a clean machine

Attempt 1:

- 10 min: `Web tests failed: ReferenceError: CustomEvent is not defined in Node.js v18`
- 15 min: `Web tests failed: require('typescript/unstable/sync') is ESM-only in TypeScript 7`
- 8 min: `Web tests failed: ReferenceError: crypto is not defined in Node.js 18 CJS files`
- 5 min: `dashboard-wiring test module list out of sync with ported code (27 problems)`
- `config-management test assertion failed: expanded row not open (pre-existing port issue)`

Attempt 2:

- 1 min: `Go compiler not installed in container; downloaded Go 1.27.0 tarball and configured GOROOT/GOPATH`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
