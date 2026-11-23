# Nano-SQL

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/only-cliches/Nano-SQL, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/nano-sql

## Pinned environment

- Project commit: `af74705e3fc4be6e65c0e4044f7dc7c5b745886c`
- Test commit: `af74705e3fc4be6e65c0e4044f7dc7c5b745886c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 5.3 to 16.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 4 | 16.1 | 2 | 2 | [run](https://argusic.com/run/ee9e04de-d604-47c6-a636-81ccb6caaeae) |
| 2 | pass | 100 | 5.5 | 5.3 | 3 | 3 | [run](https://argusic.com/run/e34e508f-7ca6-4916-b218-3e0260bb5281) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `npm install failed: sqlite3@4.0.9 native build fails on Node 18 (python: not found; then v8::ArrayBuffer::GetContents removed, no prebuilt for node-v109)`
- 1 min: `npm test failed: tests/init.ts sqlite3 v5 typings make db.all rows 'unknown', TS compile errors`

Attempt 2:

- 2 min: `sqlite3@4.0.9 failed to build from source - pre-built binary unavailable for Node 18, and source compile failed (python symlink missing, make error)`
- 1 min: `TypeScript compilation error: tests/init.ts(238) - Argument of type 'unknown' not assignable to parameter of type 'object' from newer @types/node types with sqlite3@5`
- 0.5 min: `SnapDB adapter test (05-adapters.ts) fails on repeated runs because disk-persisted _ai_store retains state; rimraf cleanup is commented out`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
