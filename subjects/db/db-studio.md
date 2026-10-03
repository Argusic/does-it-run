# db-studio

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/husamql3/db-studio, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/db-studio

## Pinned environment

- Project commit: `ef48e61ad7d9cbcf2dd0399316d39cdd9d2a35b4`
- Test commit: `ef48e61ad7d9cbcf2dd0399316d39cdd9d2a35b4`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 15.4 to 20.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 15 | 15.4 | 8 | 8 | [run](https://argusic.com/run/2d2cdb72-7157-4b5c-a0d7-9a7adcd6a759) |
| 2 | pass | 100 | 4.5 | 20.9 | 5 | 5 | [run](https://argusic.com/run/35d4bee3-e47e-481f-84b5-0ab51154b96e) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Bun runtime not pre-installed; project requires Bun >=1.2.19`
- 1 min: `bun install postinstall script from msw exited 127`
- 3 min: `Vitest startup error: rolldown uses node:util.styleText (Node 20+ API) but system Node is v18`
- 5 min: `Zod v4 import produces undefined z in vitest: import { z } from 'zod' resolves to undefined after vitest transforms modules`
- 1 min: `Server starts but crashes with SQLite connect on Bun 1.2.19 (NAPI crash with better-sqlite3)`
- `Server fails to start without a real database server running`
- 1 min: `bun run test via turbo/spawn fails because child process uses Node 18`
- `Web package vitest also fails with Node 18 for same rolldown styleText reason`

Attempt 2:

- 1.5 min: `Bun not installed in container`
- 1.5 min: `Node.js v18 too old for proxy (wrangler >Node 22)`
- 1 min: `MSW postinstall script errors in isolated linker workspace , @db-studio/monorepo workspace name resolves to garbled shell cmd`
- 0.5 min: `Bun runtime crashes on better-sqlite3 NAPI module (NAPI FATAL ERROR)`
- `Typecheck pre-existing errors: zod@4 incompatible types in @hookform/resolvers/zod (3 files, TS2769)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
