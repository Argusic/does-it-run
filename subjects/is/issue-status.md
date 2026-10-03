# issue-status

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/tadhglewis/issue-status, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/issue-status

## Pinned environment

- Project commit: `1c04c03128c19fbab73e393cb32464deb3ec8b88`
- Test commit: `1c04c03128c19fbab73e393cb32464deb3ec8b88`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 16.3 to 37.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 38 | 37.2 | 4 | 4 | [run](https://argusic.com/run/4e044356-6dfe-4817-90a8-281625dddf11) |
| 2 | pass with mocks | 92 | 15 | 16.3 | 7 | 7 | [run](https://argusic.com/run/049e035e-6b81-43c0-802b-245a6547fa96) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Node v18 is too old for Vite 8 which requires ^20.19.0 || >=22.12.0. Also @clack/core needs styleText from node:util (Node 20.12+).`
- 5 min: `tsdown@0.22.0 fails to load its config because it defaults to 'unrun' as the config loader, which is not installed. Error: Failed to import module "unrun". Please ensure it is installed.`
- 10 min: `dayjs ESM build has extensionless relative imports (e.g., import './constant' instead of './constant.js') that fail under Node's native ESM loader. When vite.config.ts uses tsx's tsImport to load the user's config file, Node loads dayjs/esm`
- 5 min: `vitest cannot start because vite.config.ts throws 'issue-status.config.ts not found' when CWD is the package directory without a config file.`

Attempt 2:

- 2 min: `Node.js v18 lacks 'node:util.styleText' required by rolldown/vitest`
- 3 min: `Missing native binding '@rolldown/binding-linux-x64-gnu' (pnpm skips optional deps in lockfile-only install)`
- 1 min: `Missing native binding '@tailwindcss/oxide-linux-x64-gnu'`
- 1 min: `Missing native binding 'lightningcss-linux-x64-gnu'`
- 2 min: `Missing tsdown peer dep 'unrun'`
- 3 min: `dayjs/esm uses extensionless relative imports rejected by Node 22 ESM resolver when loading directly from vite build`
- 2 min: `vite config requires 'issue-status.config.ts' in CWD for build step`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
