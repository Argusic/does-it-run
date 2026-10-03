# mcp-chrome

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/hangwin/mcp-chrome, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/mcp-chrome

## Pinned environment

- Project commit: `f48e71751e00bc09725c7e173423cff4f2ccd12a`
- Test commit: `f48e71751e00bc09725c7e173423cff4f2ccd12a`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 3; wall time 11.7 to 42.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | n/a | 42.3 | 0 | 0 | [run](https://argusic.com/run/3b503a2d-27fc-4d41-8163-f0bed817345e) |
| 1 | pass with mocks | 92 | 8 | 11.7 | 3 | 3 | [run](https://argusic.com/run/19319c8c-d84f-48eb-90f8-fe72512a74b0) |
| 2 | timeout | none | n/a | 42.4 | 0 | 0 | [run](https://argusic.com/run/669a96be-db5b-4b84-8502-3c4a521afedd) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `System Node.js v18.19.1 is below the project's requirement of Node >= 20, preventing pnpm install and builds`
- 2 min: `pnpm 12 blocks build scripts (better-sqlite3, esbuild, sharp, etc.) by default, failing pnpm install`
- 2 min: `Original jest.config.js with ts-jest fails to resolve .js extension imports (NodeNext module resolution) and coverage thresholds block tests from running`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
