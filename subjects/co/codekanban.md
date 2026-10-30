# CodeKanban

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/fy0/CodeKanban, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/codekanban

## Pinned environment

- Project commit: `288116bb345581d9b8f37c8bb360bf0f50b07f73`
- Test commit: `288116bb345581d9b8f37c8bb360bf0f50b07f73`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 6.5 to 6.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 7 | 6.5 | 4 | 4 | [run](https://argusic.com/run/6e56b8cb-2a22-476b-8110-94121bd53dc3) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Go 1.25+ not installed in container`
- 1 min: `Node.js v18.19.1 too old; project requires v20.19.0+ or v22.12.0+`
- 1 min: `pnpm not found`
- `corepack signature verification failed for pnpm activation`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
