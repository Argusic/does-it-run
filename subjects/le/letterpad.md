# letterpad

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/letterpad/letterpad, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/letterpad

## Pinned environment

- Project commit: `91d3e2516987ea00b1f068bda20dcd8fd14eb90d`
- Test commit: `91d3e2516987ea00b1f068bda20dcd8fd14eb90d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 39.1 to 39.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 50 | 39.1 | 4 | 4 | [run](https://argusic.com/run/b7b8e00e-b135-4364-a1d4-969186b1705c) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Bun is not installed in the container`
- 15 min: `Bun lifecycle scripts fail with '/bin/sh: Bad substitution' because dash cannot run the repo's bash [[ ]] scripts`
- 25 min: `Production build ('bun run build') is SIGKILLed by the 8GB cgroup OOM limit during Next static generation in both apps`
- 5 min: `Database seed failed with Prisma errors for missing required Author fields (bio, occupation, password)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
