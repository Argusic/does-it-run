# bento

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/nyblnet/bento, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/bento

## Pinned environment

- Project commit: `01000838496ec863ba1035eae12a8a4943020cdc`
- Test commit: `01000838496ec863ba1035eae12a8a4943020cdc`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 3; wall time 9.1 to 16.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 22 | 16.8 | 3 | 3 | [run](https://argusic.com/run/9c386144-7479-4a24-9523-b06fffaa10c3) |
| 2 | pass | 100 | 8 | 9.1 | 6 | 6 | [run](https://argusic.com/run/050348c0-9586-456f-a27f-4d4c8b246a08) |
| 3 | pass | 100 | 23 | 12.4 | 4 | 4 | [run](https://argusic.com/run/dcfa7f42-b22d-4faa-a203-a953b7c6f7bf) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Node.js 18.19.1 is too old for Vite 7 (requires node >=20.19.0 or >=22.12.0)`
- 1 min: `Installed tsx as dev dependency to run .ts test scripts`
- 1 min: `Node --experimental-strip-types required for .ts test scripts without tsx CJS/ESM cycle issues`

Attempt 2:

- 0.5 min: `test-autosave.ts fails directly from repo root - fake-indexeddb not in root node_modules`
- 0.5 min: `test-sanitize.ts fails directly - imports slides/src/model extensionless (TS bundler resolution)`
- 0.3 min: `test-slide-store.ts same extensionless-import issue`
- 0.3 min: `test-validate.ts same issue`
- 0.3 min: `test-clipboard.ts same issue`
- 0.1 min: `shell-gate.mjs called with wrong path (dist-single at root vs slides/dist-single)`

Attempt 3:

- 1 min: `Node.js v18 was too old for Vite 7 , needed ^20.19.0 || >=22.12.0`
- 3 min: `36 dash test scripts used Node 23.4+ registerHooks API`
- 1 min: `test-convert.ts spawned child processes without --experimental-strip-types`
- `test-dash-steps.ts memory probe needs --expose-gc , pre-existing limitation with this Node version`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
