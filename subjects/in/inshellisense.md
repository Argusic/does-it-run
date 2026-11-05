# inshellisense

**Verdict: runs.** Argusic Score 95 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/microsoft/inshellisense, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/inshellisense

## Pinned environment

- Project commit: `63872c52ebc83389735998ade5486f1bd069d0bf`
- Test commit: `63872c52ebc83389735998ade5486f1bd069d0bf`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 5.2 to 47.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 90 | 8 | 5.2 | 2 | 1 | [run](https://argusic.com/run/34d8b0e0-f4bd-4678-8088-4c9def748d87) |
| 2 | pass | 100 | 2 | 47.7 | 6 | 6 | [run](https://argusic.com/run/22ecbe7d-cb98-4b13-9d1e-62ab021e2f44) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `node:sea static import fails on Node 18`
- 2 min: `@microsoft/tui-test requires Node >=20 for native binary`

Attempt 2:

- 6 min: `Jest suite failed: 'No such built-in module: node:sea' when src/utils/node.ts imported node:sea statically on Node v18.19.1`
- 3 min: `npm run test:e2e failed with 'Cannot find module @microsoft/tui-test-linux-x64-gnu' because the optional native package was not installed`
- 4 min: `npm link failed with EACCES writing to root-owned /usr/local`
- 22 min: `Full e2e suite produced no output and timed out because it also spawns fish and zsh, which are not installed in this container`
- 5 min: `e2e color assertion failed: expected bg #7d56f4 but terminal reported #8787ff (chalk downgraded truecolor)`
- 4 min: `'proper overflow truncation in command' e2e test timed out when run concurrently, reporting only 'do' typed`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
