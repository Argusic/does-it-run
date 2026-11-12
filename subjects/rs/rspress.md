# rspress

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/web-infra-dev/rspress, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/rspress

## Pinned environment

- Project commit: `eef4b4dba1e00ffed92ae96d1f9a7a792d394f7d`
- Test commit: `eef4b4dba1e00ffed92ae96d1f9a7a792d394f7d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 21.9 to 32.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 25 | 32.5 | 3 | 3 | [run](https://argusic.com/run/b4edbccd-7031-4039-afa2-4c210a6063c1) |
| 2 | pass | 100 | 15 | 21.9 | 3 | 3 | [run](https://argusic.com/run/66a75343-f6cc-4ddb-9311-22c773d77b95) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Node v18.19.1 is installed but project requires >=22.12`
- 3 min: `pnpm not installed and npm install -g fails due to permissions on /usr/local`
- 17 min: `Build fails with ERR_UNKNOWN_FILE_EXTENSION for .ts config files; tests fail with ERR_UNKNOWN_FILE_EXTENSION for .tsx files`

Attempt 2:

- 5 min: `Project .nvmrc requires Node.js v24.13.0 but the container had v18.19.1`
- 5 min: `rstack CLI could not load rstack.config.ts files (ERR_UNKNOWN_FILE_EXTENSION .ts) because process.features.typescript is false without --experimental-strip-types`
- 3 min: `pnpm install's prepare script triggered a recursive nx build that referenced the old Node version at /home/runner/.nvm/versions/node/v22.14.0/bin/node`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
