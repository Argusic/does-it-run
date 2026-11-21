# WeWorker

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/WeWorker/WeWorker, licensed Apache-2.0, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/weworker

## Pinned environment

- Project commit: `2a8ed5aafc17821c2cd97c4030b41dc40ffee3b0`
- Test commit: `2a8ed5aafc17821c2cd97c4030b41dc40ffee3b0`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 16.1 to 16.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 16 | 16.1 | 3 | 3 | [run](https://argusic.com/run/41eb8ca0-7d95-4935-b8c5-9099e2366297) |

## What was observed on a clean machine

Attempt 1:

- `Pre-built Node.js v22.12.0 binary lacks SQLite FTS5 module (compile-time option), causing 41 backend-ts memory-store tests to fail with 'no such module: fts5'`
- `3 cancelled tests in electron/__tests__/dedicated-browser.test.mjs due to flaky async cancellation timing (cancelledByParent)`
- 5 min: `5 test failures in renderer/src/__tests__/desktop-d10-d12-regressions.test.js: D11 tests could not find internal helper functions (normalizeWeekdays, weekdayField); D12 tests referenced non-existent renameResourceHints and outdated markdown`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
