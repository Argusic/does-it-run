# qwengate

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/youssefvdel/qwengate, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/qwengate

## Pinned environment

- Project commit: `5220f7d3c50c2d9538ec3d6d393aed4f13369950`
- Test commit: `5220f7d3c50c2d9538ec3d6d393aed4f13369950`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 20 to 20 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 45 | 20 | 3 | 3 | [run](https://argusic.com/run/e0cf29ff-73cf-440a-9c40-17c7353d2302) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `bun.sh installer failed: unzip not installed and no root`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
