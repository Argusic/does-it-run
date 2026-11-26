# WikiDocs

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Zavy86/WikiDocs, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/wikidocs

## Pinned environment

- Project commit: `7fd85bf834d5c10695db075ff022a7c2dd5b46c3`
- Test commit: `7fd85bf834d5c10695db075ff022a7c2dd5b46c3`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 5.9 to 6.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 7 | 6.9 | 2 | 2 | [run](https://argusic.com/run/9ec73ca5-41a1-417a-9eb2-059ce28f186c) |
| 2 | pass | 100 | 5 | 5.9 | 1 | 1 | [run](https://argusic.com/run/443f436c-fb6d-433c-a0dd-f6e425f01db3) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Angular CLI requires Node.js v22.22.3+ but container has v18.19.1`
- `Desktop Electron requires --no-sandbox flag and dbus is unavailable in container`

Attempt 2:

- 4 min: `System Node 18.19.1 is too old for this project. NestJS 11 and Angular 22 require Node 20+ (Angular 22 needs >=22.22.3). npm ci succeeds with warnings, but tests and frontend build fail at runtime.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
