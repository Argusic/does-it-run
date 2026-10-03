# drawnix

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/plait-board/drawnix, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/drawnix

## Pinned environment

- Project commit: `b138ff867943ddff6c4c79560e10ab6ee3b5600e`
- Test commit: `b138ff867943ddff6c4c79560e10ab6ee3b5600e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 4.2 to 4.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 4.2 | 1 | 1 | [run](https://argusic.com/run/f787f735-9e61-4e3b-9986-5011a0bb2150) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node.js v18.19.1 is too old , the project requires v20.20.2 (per .nvmrc) and many deps fail engine checks`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
