# hyper-fetch

**Verdict: runs.** Argusic Score 97.5 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/BetterTyped/hyper-fetch, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/hyper-fetch

## Pinned environment

- Project commit: `f2baf196d7921a50abe6eec73413e3027a820f6a`
- Test commit: `f2baf196d7921a50abe6eec73413e3027a820f6a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 24.9 to 41.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 26 | 24.9 | 4 | 4 | [run](https://argusic.com/run/48895cc2-9165-4c11-a5fd-a82b73ffe240) |
| 2 | pass | 95 | 18 | 41.9 | 4 | 3 | [run](https://argusic.com/run/41e2f656-ec67-49c2-ac55-f4af21fd96ea) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `pnpm not found in PATH`
- 5 min: `Node v18 lacks styleText (Vite 8 requirement)`
- 2 min: `install-peers.js crashes on ESM-only chalk v5`
- 3 min: `GraphQL adapter tests fail: CloseEvent not defined in Node 22`

Attempt 2:

- 1 min: `install-peers.js uses require('chalk') but chalk v5 is ESM-only - prepare script fails under pnpm`
- 2 min: `Node 18.19.1 is too old for Vite 8 (needs 20.19+ or 22.12+)`
- 2 min: `CloseEvent not defined in Node.js 22 - ControlledWebSocket in adapter-graphql tests fails`
- 1 min: `Bun not available - elysia __bun__/ tests cannot run`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
