# ShiguReader

**Verdict: runs.** Argusic Score 86.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/hjyssg/ShiguReader, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/shigureader

## Pinned environment

- Project commit: `480ef403493a75092a7a9249328cf472fff88573`
- Test commit: `480ef403493a75092a7a9249328cf472fff88573`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 4.3 to 4.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 86.67 | 2 | 4.3 | 3 | 1 | [run](https://argusic.com/run/7d83d5f8-b0bf-4f9d-a667-c7af76960ca7) |

## What was observed on a clean machine

Attempt 1:

- `packages/backend/pathUtil.test.js: 10 tests fail on Linux , tests use Windows path conventions (C:\..., Y:\...)`
- `packages/frontend/sender.test.js: 4 tests fail , ESM import in Sender.js not transpiled for CJS mocha runner`
- `packages/name-parser: mocha missing from devDependencies`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
