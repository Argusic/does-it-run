# WA-AKG

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/mrifqidaffaaditya/WA-AKG, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/wa-akg

## Pinned environment

- Project commit: `c7dd01a04339e4363b549beb3a41fe02cf131acb`
- Test commit: `c7dd01a04339e4363b549beb3a41fe02cf131acb`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 12.2 to 12.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 12.2 | 6 | 6 | [run](https://argusic.com/run/705c00e2-e89f-4944-9dff-600afb165059) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `npm install failed: @whiskeysockets/baileys requires Node.js 20+, container had Node 18.19.1`
- 8 min: `No database server in container; project requires MySQL/PostgreSQL (Prisma datasource mysql)`
- 4 min: `MySQL 8.0.36 (Ubuntu debs, extracted) repeatedly SIGSEGVed in this container`
- 1 min: `Initial app launch logged Prisma errors (DB unreachable / table missing) because the earlier MySQL server had crashed`
- 1 min: `No automated test suite exists: no npm test script, no test runner in package.json`
- 1 min: `login page (auth route) requires a CSRF token for the NextAuth credentials callback`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
