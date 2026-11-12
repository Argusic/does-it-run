# dsh-purge

**Verdict: runs with mocks.** Argusic Score 86 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/mmparko/dsh-purge, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/run/c2993538-4532-407c-805f-49df0af60e0f

## Pinned environment

- Project commit: `033e6bd1e0f101352b39075ecd0d758ffef26b76`
- Test commit: `033e6bd1e0f101352b39075ecd0d758ffef26b76`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 1.7 to 2.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 0.5 | 2.2 | 1 | 1 | [run](https://argusic.com/run/c2993538-4532-407c-805f-49df0af60e0f) |
| 2 | pass with mocks | 92 | 2 | 1.7 | 2 | 2 | [run](https://argusic.com/run/e631b2ca-5cf1-4402-a0b6-89c579b7558a) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `3 redteam modules (store, tools, ui) depend on node:sqlite which requires Node.js 22+. Not available on Node 18.`

Attempt 2:

- `node:sqlite not available in Node.js 18; script export-engagement-report.mjs fails to import`
- `npm global install blocked by EACCES (no root)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
