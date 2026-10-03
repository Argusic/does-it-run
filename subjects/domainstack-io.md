# domainstack.io

**Verdict: runs.** Argusic Score 93.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/jakejarvis/domainstack.io, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/domainstack-io

## Pinned environment

- Project commit: `88b8831009b82dc1f86531239fdfb28bbbe6a7a0`
- Test commit: `88b8831009b82dc1f86531239fdfb28bbbe6a7a0`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, no run possible
- Valid runs: 4; wall time 14.4 to 87.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 6.5 | 27.9 | 4 | 4 | [run](https://argusic.com/run/e1378a2f-0f7a-41a0-b679-ca65cf64ee4f) |
| 1 | timeout | none | n/a | 87.1 | 0 | 0 | [run](https://argusic.com/run/36c13084-fbfd-4768-94fa-da2af186b4e3) |
| 2 | pass | 86.67 | 2 | 14.4 | 3 | 1 | [run](https://argusic.com/run/8270eaa0-cd5a-4501-af35-8dc9269f2ce5) |
| 3 | timeout | none | n/a | 87.2 | 0 | 0 | [run](https://argusic.com/run/e021d2b1-d34f-4538-9892-423a691a069e) |

## What was observed on a clean machine

Attempt 1:

- 2.3 min: `System Node.js is v18.19.1 but project requires >=24`
- 0.7 min: `Puppeteer postinstall failed - no unzip binary to extract Chrome`
- 0.5 min: `Build failed: auth module requires at least one OAuth provider configured at build time`
- 2.1 min: `Web app browser tests required Playwright/Chromium but browsers were not installed`

Attempt 2:

- 2 min: `Node.js v18 was installed but the project requires >=24. Installed v24.20.0 via nvm.`
- 1 min: `Puppeteer postinstall failed to download Chrome (missing unzip/tar.exe). Not a build blocker.`
- 1 min: `Playwright browser tests (35 .test.tsx files) cannot run: no root access to install system deps.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
