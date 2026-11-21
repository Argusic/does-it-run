# ui

**Verdict: runs.** Argusic Score 97.5 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/vercel-labs/ui, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/ui

## Pinned environment

- Project commit: `220c1a0d7278872286a620a8e4ee4210ca46f9bd`
- Test commit: `220c1a0d7278872286a620a8e4ee4210ca46f9bd`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 16.1 to 46.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8 | 46.8 | 6 | 6 | [run](https://argusic.com/run/b9ce78b6-e2a7-434a-b63d-b2e3f1b96618) |
| 2 | pass | 95 | 3 | 16.1 | 4 | 3 | [run](https://argusic.com/run/5e4a727b-3c29-47c8-b0be-32589469ffa1) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `System Node.js v18.19.1 too old for @sveltejs/vite-plugin-svelte (needs node:util.styleText)`
- 1 min: `Built-in pnpm not available - corepack not installed`
- 1 min: `pnpm install initially succeeded with Node v18 but svelte build failed due to @sveltejs/vite-plugin-svelte needing node:util.styleText`
- 2 min: `core unit tests exited 1 due to 96 unhandled errors from jsdom/undici incompatibility with Node v18 (webidl.util.markAsUncloneable)`
- 1 min: `svelte package build failed: rolldown could not find native binding for linux-x64-gnu`
- `Playwright e2e tests timed out with 33 parallel workers on 2-core machine`

Attempt 2:

- 0.5 min: `pnpm not found in PATH (Node 18 ships without it)`
- 1 min: `Node 18 lacks styleText in node:util needed by @sveltejs/vite-plugin-svelte`
- 1 min: `rolldown optional native binding @rolldown/binding-linux-x64-gnu not installed after Node upgrade`
- `check-comments.mjs lint fails: git merge-base HEAD origin/main fails in detached HEAD`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
