# AI-Engineering-Coach

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/microsoft/AI-Engineering-Coach, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/ai-engineering-coach

## Pinned environment

- Project commit: `74eb09ca71078804611142da12402016441fc1bb`
- Test commit: `74eb09ca71078804611142da12402016441fc1bb`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 8.3 to 30.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8 | 8.3 | 1 | 1 | [run](https://argusic.com/run/59cee494-6a7c-4fe7-9369-6aad68767468) |
| 2 | pass with mocks | 92 | 6 | 30.3 | 5 | 5 | [run](https://argusic.com/run/f0c921b1-921f-46a2-828c-9cd743709c5c) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `npm test fails: 7 tests in github-app-analytics.test.ts fail with 'status' expected 'ready' got 'unavailable' because the production default query() calls the missing sqlite3 CLI binary, but the test creates databases via Node's built-in Da`

Attempt 2:

- 1 min: `system Node was v18.19.1 but project requires Node >= 20 (CI uses 22)`
- 2 min: `7 unit tests failed: analyzer shells out to missing sqlite3 CLI (spawn sqlite3 ENOENT)`
- `playwright browser missing (e2e aborts)`
- `npm run smoke-test fails: bundle requires 'vscode' module outside host`
- `VS Code extension host did not activate the installed extension in this container (no onCommand: activation reached); SUID sandbox also blocks root-less code launch`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
