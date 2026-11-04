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
- Valid runs: 2; wall time 8.5 to 15.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 13 | 15.1 | 2 | 2 | [run](https://argusic.com/run/2f52a233-1c65-4e2c-b8a8-140361ee3178) |
| 2 | pass | 100 | 6 | 8.5 | 2 | 2 | [run](https://argusic.com/run/8d7557f3-8ac5-4e32-8bed-624b18e4e117) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `System Node.js is v18.19.1 but project requires ^22.22.3 || >=24.8.0; pnpm not installed`
- 1 min: `Build script 'node scripts/prepare-build.ts' fails on Node 26 , unknown file extension .ts`

Attempt 2:

- 1 min: `Node v18.19.1 too old; project requires ^22.22.3 or >=24.8.0. First build failed with ERR_UNKNOWN_FILE_EXTENSION for .ts files.`
- 2 min: `vitest failed at startup: missing native binding @rolldown/binding-linux-x64-gnu, an optional dependency of rolldown that never resolved.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
