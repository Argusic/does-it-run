# vue-quill

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/vueup/vue-quill, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/vue-quill

## Pinned environment

- Project commit: `8d327c5f209f1f998a2e8d944b11035346d7e0c6`
- Test commit: `8d327c5f209f1f998a2e8d944b11035346d7e0c6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 5 to 13.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 10 | 13.9 | 3 | 3 | [run](https://argusic.com/run/05fb5b2e-d0da-4535-b4d2-1599a642dc45) |
| 2 | pass | 100 | 5 | 5 | 4 | 4 | [run](https://argusic.com/run/13fb470f-2f65-42b4-96ef-54968e79a9dc) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `chalk v5 ESM-only: scripts/chalk.js require() of ESM chalk failed`
- 1 min: `serialize-javascript crypto is not defined in rollup on Node 18`
- 0.5 min: `quill and quill-delta dependencies not installed for workspace package`

Attempt 2:

- 2 min: `Node.js v18.19.1 does not satisfy package engine requirement >=22.22.1`
- 1 min: `chalk v5 is ESM-only but build scripts (chalk.js, logger.ts) use require()`
- 1 min: `Rollup build fails due to missing quill and quill-delta in root node_modules (they were only in packages/vue-quill/node_modules)`
- 1 min: `TypeScript test files (.ts) cannot be run directly with older Node; need --experimental-strip-types`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
