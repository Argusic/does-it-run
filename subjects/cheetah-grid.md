# cheetah-grid

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/future-architect/cheetah-grid, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/cheetah-grid

## Pinned environment

- Project commit: `28ae0aae380ae576d056912af95645ac97a003ea`
- Test commit: `28ae0aae380ae576d056912af95645ac97a003ea`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 11.6 to 12.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 11.6 | 4 | 4 | [run](https://argusic.com/run/62e95d57-031a-4390-bbe8-4bc64a7087b0) |
| 2 | pass | 100 | 7 | 12.9 | 4 | 4 | [run](https://argusic.com/run/26cb3ecb-f682-470c-a103-78ba264e9f33) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node v18.19.1 too old for rolldown@1.2.4 native bindings which require Node>=20.19`
- 1 min: `pnpm not available on Node 18 (no corepack, no pnpm)`
- 2 min: `rolldown@1.2.4 optional native binding @rolldown/binding-linux-x64-gnu not installed`
- 3 min: `vitest browser tests failed: Chromium distribution chrome not found at /opt/google/chrome/chrome`

Attempt 2:

- 1 min: `Node.js v18.19.1 lacks 'styleText' from node:util (needs ≥20.12.0) used by rolldown/tsdown`
- 1 min: `Vitest config defaulted browser channel to 'chrome', requiring system Chrome at /opt/google/chrome/chrome`
- `7 visual screenshot tests failed in CheckColumn_spec.js and CheckStyle_spec.js due to pixel mismatches in checkbox rendering between Playwright's bundled Chrome v148 and the expected snapshots`
- `packages/cheetah-grid-playwright build fails , missing 'unrun' dependency`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
