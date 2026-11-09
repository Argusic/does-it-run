# jira.js

**Verdict: runs.** Argusic Score 90 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/MrRefactoring/jira.js, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/jira-js

## Pinned environment

- Project commit: `392900765d4ed629ec232b788e6ad3c7b0229ac8`
- Test commit: `392900765d4ed629ec232b788e6ad3c7b0229ac8`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 4.6 to 6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 6 | 6 | 3 | 3 | [run](https://argusic.com/run/0c1a43a6-5766-4785-9d54-ead394a92ed5) |
| 2 | pass | 100 | 8 | 4.6 | 0 | 0 | [run](https://argusic.com/run/ffd64df6-0964-409b-9e3a-95319da7626d) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Container had Node 18 but project requires Node >=22`
- 1 min: `pnpm (required by project) was missing`
- 3 min: `4 test failures in schemaAuditReport.test.ts: Node 22 requires --experimental-strip-types to spawn .ts files, and the test used process.execPath to invoke a .ts script without the flag, causing ENOENT on the report file`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
