# lcu

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/amontlabs/lcu, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/lcu

## Pinned environment

- Project commit: `748303e9315eea4f1877413bd69f00cb270e3d12`
- Test commit: `748303e9315eea4f1877413bd69f00cb270e3d12`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 7.1 to 11.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 44 | 7.1 | 2 | 2 | [run](https://argusic.com/run/0cae5d53-24d4-46f6-8896-2e4388ba6346) |
| 2 | pass with mocks | 92 | 7.5 | 11.4 | 3 | 3 | [run](https://argusic.com/run/8c857cb6-bdbc-4873-bc79-079e4ae6ba9b) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `npm adapter tests: 4 Node 18 MockTimers.enable signature mismatches`
- `npm adapter tests: 3 test files require OMP/Pi harness installations`

Attempt 2:

- `MockTimers.enable in Node 18 expects 'timers' as an Array, used in adapters/test/client.test.mjs (4 tests fail)`
- `Node 18 cannot load .ts ESM files, causing adapters/test/omp.test.mjs, pi-approval.test.mjs, pi.test.mjs to fail`
- `MCP server exits on mock app because stub node binary exits immediately`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
