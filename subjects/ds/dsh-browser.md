# dsh-browser

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/omdsh-dev/dsh-browser, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/dsh-browser

## Pinned environment

- Project commit: `36fd3ad2d22b814d462b158541c843e6df0bb1cd`
- Test commit: `36fd3ad2d22b814d462b158541c843e6df0bb1cd`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 27.8 to 27.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 18.5 | 27.8 | 4 | 4 | [run](https://argusic.com/run/600f9549-b701-4b32-931b-8bb27329f582) |

## What was observed on a clean machine

Attempt 1:

- 0.8 min: `Node.js v18 too old (needs ^22.19)`
- 0.4 min: `pnpm not found`
- 4 min: `rsync not found; installer requires it`
- `No Chrome browser in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
