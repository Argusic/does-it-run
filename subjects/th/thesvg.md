# thesvg

**Verdict: runs.** Argusic Score 97.5 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/glincker/thesvg, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/thesvg

## Pinned environment

- Project commit: `fa87032438a21826df5a4fbb0e6b0ce9d02147d6`
- Test commit: `fa87032438a21826df5a4fbb0e6b0ce9d02147d6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 3.1 to 5.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 95 | 12 | 3.1 | 4 | 3 | [run](https://argusic.com/run/a5b7f4a5-dc31-4dc3-8965-4ae187a7f404) |
| 2 | pass | 100 | 6 | 5.5 | 4 | 4 | [run](https://argusic.com/run/8bc96776-799e-4a0f-84e5-482925856ee8) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `pnpm lockfile supply-chain policy violation due to stale lockfile`
- 3 min: `Node 18.19 too old for rolldown/vitest (needs node:util styleText)`
- 1 min: `Missing @rolldown/binding-linux-x64-gnu native binding (optional dep not pulled by pnpm)`
- `pnpm.overrides in package.json ignored by pnpm 12 (non-fatal warning)`

Attempt 2:

- 0.5 min: `pnpm not installed globally - EACCES on npm install -g`
- 1 min: `pnpm 12.x rejects ignored build scripts (core-js, esbuild, unrs-resolver, workerd)`
- 1 min: `pnpm.overrides in package.json not supported by pnpm 12.x - caused out-of-sync lockfile on test run`
- 1 min: `Node 18 too old for rolldown/vitest - node:util.styleText not available`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
