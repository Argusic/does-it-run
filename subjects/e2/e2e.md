# e2e

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/tester-army/e2e, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/e2e

## Pinned environment

- Project commit: `fd3a0c766b4d40c74fabdbc578e3832d80553bf9`
- Test commit: `fd3a0c766b4d40c74fabdbc578e3832d80553bf9`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 15.1 to 15.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 13 | 15.1 | 2 | 2 | [run](https://argusic.com/run/2f52a233-1c65-4e2c-b8a8-140361ee3178) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `System Node.js is v18.19.1 but project requires ^22.22.3 || >=24.8.0; pnpm not installed`
- 1 min: `Build script 'node scripts/prepare-build.ts' fails on Node 26 , unknown file extension .ts`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
