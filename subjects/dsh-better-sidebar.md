# DSH-better-sidebar

**Verdict: runs with mocks.** Argusic Score 56 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/omdsh-dev/DSH-better-sidebar, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/dsh-better-sidebar

## Pinned environment

- Project commit: `1499502bfa63c8724070eef10dba5fa15b659a97`
- Test commit: `1499502bfa63c8724070eef10dba5fa15b659a97`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 40.2 to 77.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 40.2 | 0 | 0 | [run](https://argusic.com/run/f09405f0-1f4a-4946-9c10-cb4314fbadd6) |
| 2 | pass with mocks | 92 | 25 | 77.2 | 5 | 5 | [run](https://argusic.com/run/c3d11dc0-61bd-44db-a544-a4ae1acae00a) |

## What was observed on a clean machine

Attempt 2:

- 5 min: `Node.js v18 did not satisfy pnpm 11 requirement (>=22.13); pnpm 9 used instead then Node upgraded via 'n' to v22`
- 1 min: `git identity not configured, causing revert/cherry-pick tests to fail`
- 2 min: `Japanese locale file missing pluginMnemeName and pluginMnemeDesc keys, key-set equality test failed`
- 5 min: `All 18 non-zh locale files missing 6 keys each (pluginAgentPersonaName, pluginAgentPersonaDesc, pluginTylinaName, pluginTylinaDesc, pluginMnemeName, pluginMnemeDesc)`
- `market-manifest pack test very slow (288s) and plugin-meta pack test also slow; E2E tests need real DSH host`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
