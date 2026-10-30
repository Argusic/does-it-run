# Cliparr

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/TechSquidTV/Cliparr, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/cliparr

## Pinned environment

- Project commit: `9cc203d863539f96472bc6e4f189b391e43e9827`
- Test commit: `9cc203d863539f96472bc6e4f189b391e43e9827`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 5.2 to 5.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 6 | 5.2 | 5 | 5 | [run](https://argusic.com/run/5717ff87-c106-4f4c-893b-84b6d6bec5d5) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Node v18.19.1 is installed but the project requires Node >=24.16.0`
- 1 min: `npm install -g n failed with EACCES mkdir /usr/local/lib/node_modules/n`
- 1 min: `pnpm not found on PATH`
- 1 min: `No .env file present, so APP_KEY was unset`
- 1 min: `No Playwright browser installed`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
