# grok-cli

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/superagent-ai/grok-cli, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/grok-cli

## Pinned environment

- Project commit: `fb97af83f06dca873281d60168430f06c8de6324`
- Test commit: `fb97af83f06dca873281d60168430f06c8de6324`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 3; wall time 8.5 to 13.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 7.9 | 8.5 | 2 | 2 | [run](https://argusic.com/run/6664b951-16a8-4a97-8c98-e06ec9071490) |
| 2 | pass with mocks | 92 | 14 | 13.8 | 4 | 4 | [run](https://argusic.com/run/8407e206-eb14-4208-95c7-8aca38d8e657) |
| 3 | pass with mocks | 92 | 8 | 8.7 | 3 | 3 | [run](https://argusic.com/run/6ac79a23-1866-4096-808f-888379336284) |

## What was observed on a clean machine

Attempt 1:

- `78/452 tests failed due to vi.stubGlobal/vi.resetModules/vi.unstubAllGlobals not being available in Bun's test runner (Vitest-specific APIs)`
- `CLI imports package.json without import attribute, causing ERR_IMPORT_ASSERTION_TYPE_MISSING on Node.js 18`

Attempt 2:

- 2 min: `Bun not installed (unzip missing for install.sh, npm global install fails without --prefix)`
- 4 min: `Node.js 18 too old , vitest 4.x requires styleText from node:util (Node 20+)`
- 7 min: `bun:sqlite built-in not available when vitest runs under Node`
- 1 min: `Built CLI fails with ERR_MODULE_NOT_FOUND under node (uses Bun-native module resolution)`

Attempt 3:

- 2 min: `Node.js 18 lacks node:util.styleText required by vitest 4, causing test runner crash`
- 3 min: `bun:sqlite not available when vitest runs under Node.js, causing 1 test file to fail`
- 1 min: `TS4053 type error in shim: BetterSqlite3.Transaction not exposed`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
