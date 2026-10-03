# AI-Engineering-Coach

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/microsoft/AI-Engineering-Coach, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/ai-engineering-coach

## Pinned environment

- Project commit: `74eb09ca71078804611142da12402016441fc1bb`
- Test commit: `74eb09ca71078804611142da12402016441fc1bb`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 8.3 to 8.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8 | 8.3 | 1 | 1 | [run](https://argusic.com/run/59cee494-6a7c-4fe7-9369-6aad68767468) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `npm test fails: 7 tests in github-app-analytics.test.ts fail with 'status' expected 'ready' got 'unavailable' because the production default query() calls the missing sqlite3 CLI binary, but the test creates databases via Node's built-in Da`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
