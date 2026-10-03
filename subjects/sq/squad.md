# squad

**Verdict: runs.** Argusic Score 90 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/bradygaster/squad, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/squad

## Pinned environment

- Project commit: `fcb7747c7a0152230b03603850006447d5422d1f`
- Test commit: `fcb7747c7a0152230b03603850006447d5422d1f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 27.3 to 27.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 90 | 26 | 27.3 | 6 | 3 | [run](https://argusic.com/run/58d4564c-2b81-4151-956d-8b30e67468cd) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `System Node.js v18.19.1 below project minimum >=22.5.0`
- 2 min: `npm internal error with Node v22.5.0 , packages require >=22.12 or >=22.18 (eslint, vite, cspell-lib)`
- 5 min: `Second 'npm install' broke workspace resolution , replaced workspace symlinks with stale npm copies missing required SDK exports`
- `gh-aw-* tests fail , require 'gh aw' CLI extension ('gh extension install github/gh-aw') not available in this environment`
- `repl-ux and layout-anchoring terminal spinner tests fail , require interactive PTY, non-interactive CI terminal cannot render spinner characters`
- `resolution.test.ts fails due to test-model pollution from prior squad init run , personal squad config persists across runs`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
