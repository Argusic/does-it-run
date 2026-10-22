# life-kline

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/miounet11/life-kline, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/life-kline

## Pinned environment

- Project commit: `7abf184df370452ee8279d72c8b45bc09e19913b`
- Test commit: `7abf184df370452ee8279d72c8b45bc09e19913b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 7.4 to 7.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 7 | 7.4 | 2 | 2 | [run](https://argusic.com/run/75a19bc2-fa20-40f9-a774-18dd6c39aa40) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `npm install failed with ERESOLVE peer dependency conflict on react-helmet-async with React 19`
- 2 min: `createUserProfile in database.js: 16 SQL placeholders for 15 columns`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
