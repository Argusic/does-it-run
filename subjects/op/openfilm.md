# openfilm

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/openfilm/openfilm, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/openfilm

## Pinned environment

- Project commit: `6de41abd8326658dd07952d01cebdf6282510ec5`
- Test commit: `6de41abd8326658dd07952d01cebdf6282510ec5`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 20.9 to 20.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 20.9 | 5 | 5 | [run](https://argusic.com/run/020d6225-0dcc-484c-b98f-92515133a554) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node 18.19.1 installed but project requires >=22.18`
- 1 min: `pnpm not available, corepack signature verification failed`
- 2 min: `Playwright browsers not installed`
- 1 min: `tsx (--import tsx) not resolvable from workspace packages`
- 1 min: `Test command missing --import tsx flag for .ts test files`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
