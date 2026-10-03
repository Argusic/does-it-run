# buildawesome

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/11ty/buildawesome, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/buildawesome

## Pinned environment

- Project commit: `cdc06972c45d62f0f99a5c6b1354d820faaae315`
- Test commit: `cdc06972c45d62f0f99a5c6b1354d820faaae315`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 20.4 to 20.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1.5 | 20.4 | 4 | 4 | [run](https://argusic.com/run/cdd087e3-5e2b-4311-849b-a1451930aaf3) |

## What was observed on a clean machine

Attempt 1:

- 1.5 min: `Node.js 18.19.1 below required >=22.15`
- 0.5 min: `npm install failed on simple-git-hooks script`
- 2 min: `spawnAsync rejected on stderr warnings from experimental-strip-types`
- 1 min: `18 test failures from TypeScript extension expectations`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
