# dsh-purge

**Verdict: runs with mocks.** Argusic Score 67.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/YuJunZhiXue/dsh-purge, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/dsh-purge

## Pinned environment

- Project commit: `24710ff2d10c9bc54ea418713ac1299ad4cb0180`
- Test commit: `24710ff2d10c9bc54ea418713ac1299ad4cb0180`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 12.4 to 14.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 43.33 | 0.5 | 14.2 | 3 | 2 | [run](https://argusic.com/run/6d203f0f-aea5-4404-a164-379bf6735622) |
| 2 | pass with mocks | 92 | 2 | 12.4 | 0 | 0 | [run](https://argusic.com/run/e9c61450-2e8a-4dd4-b65a-4f836904e397) |

## What was observed on a clean machine

Attempt 1:

- `3 redteam modules fail to import due to node:sqlite not available in Node 18`
- `no test suite exists in the repository`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
