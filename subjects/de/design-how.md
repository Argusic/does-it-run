# design.how

**Verdict: runs.** Argusic Score 93.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/arla6ka/design.how, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/design-how

## Pinned environment

- Project commit: `c0f7df5116fc91de6dc258157003c6440249f25e`
- Test commit: `c0f7df5116fc91de6dc258157003c6440249f25e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 11.6 to 11.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 93.33 | 11 | 11.6 | 3 | 2 | [run](https://argusic.com/run/d65a246e-82b2-4877-8930-ea67ac04e314) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Python dependencies fonttools, brotli, uharfbuzz, numpy, pillow not installed`
- 2 min: `Playwright and Chromium browser not installed`
- `make-motion template requires Node >=22.6, environment has v18.19.1`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
