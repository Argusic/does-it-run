# electric-pglite

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/neondatabase/electric-pglite, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/electric-pglite

## Pinned environment

- Project commit: `dbd6eb41c9aca5b655adf0f516c3c9888469a02c`
- Test commit: `dbd6eb41c9aca5b655adf0f516c3c9888469a02c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 7.7 to 16.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 15 | 7.7 | 5 | 5 | [run](https://argusic.com/run/ee887458-e71a-4a06-925b-191ae4e51998) |
| 2 | pass | 100 | 18 | 16.1 | 4 | 4 | [run](https://argusic.com/run/476aed08-0bbd-4a67-9856-81f2c5ecf216) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node.js v18 installed but >=20 required by package`
- 1 min: `pnpm not found on PATH`
- 1 min: `better-sqlite3 native build failed (node-gyp undici incompatibility)`
- 2 min: `postgres-pglite git submodule could not be cloned (auth required)`
- 1 min: `Workspace dependency packages not built`

Attempt 2:

- 1 min: `pnpm 9.7.0 not on PATH (npm global install needs root)`
- 3 min: `postgres-pglite git submodule empty; Docker unavailable to build WASM from source`
- 3 min: `Extension packages (pglite-age, pglite-tools, pglite-icu-full) fail to build , they need their own release WASM files`
- 5 min: `Node.js v18.19.1 below required >=20`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
