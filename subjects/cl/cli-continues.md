# cli-continues

**Verdict: runs.** Argusic Score 96.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/yigitkonur/cli-continues, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/cli-continues

## Pinned environment

- Project commit: `e486cd22a592d89d890cff056624647fbe9cbe80`
- Test commit: `e486cd22a592d89d890cff056624647fbe9cbe80`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 6.6 to 7.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 93.33 | 6 | 7.7 | 3 | 2 | [run](https://argusic.com/run/90f2214f-8f04-4857-a1f2-a28d465af2e5) |
| 2 | pass | 100 | 10 | 6.6 | 4 | 4 | [run](https://argusic.com/run/3809dbef-cb1c-4014-bd70-1ec39d685716) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `System Node.js v18.19.1 does not satisfy project requirement of Node >=22.5.0`
- 1 min: `pnpm 12.3.4 blocked esbuild@0.27.2 postinstall script due to build-script approval policy`
- `pnpm run lint reports 3 pre-existing Biome errors (2 noUselessConstructor in src/errors.ts, 1 noExplicitAny in src/__tests__/e2e-conversions.test.ts) , these are pre-existing source issues, not install blockers`

Attempt 2:

- 2 min: `Node.js v18.19.1 lacks node:sqlite (needs >=22.5)`
- 1 min: `pnpm not available on PATH`
- 1 min: `pnpm blocked esbuild postinstall`
- 1 min: `Biome lint errors in test files`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
