# ai-video-editor

**Verdict: could not verify.** Argusic Score 80 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/MartinDelophy/ai-video-editor, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/ai-video-editor

## Pinned environment

- Project commit: `68980d142cce421eab86cd4ef26a4475a6affd56`
- Test commit: `68980d142cce421eab86cd4ef26a4475a6affd56`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 3; wall time 2.9 to 10.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 1 | 2.9 | 1 | 1 | [run](https://argusic.com/run/2c28363e-2744-44a9-85b3-b21945d37603) |
| 2 | fail | 80 | 3 | 10.7 | 1 | 1 | [run](https://argusic.com/run/2cbab703-9d50-442a-ac71-0f13eadb1961) |
| 2 | fail | 80 | 19 | 8.7 | 1 | 1 | [run](https://argusic.com/run/4781328e-8a8b-4eb5-ba27-0a35e3a2512f) |

## What was observed on a clean machine

Attempt 1:

- `Node.js v18 detected (requires v20+ per README). ESLint 10 fails with 'util.styleText is not a function'`

Attempt 2:

- 2 min: `npm run check fails - ESLint 10 requires Node.js 20+ for util.styleText in stylish formatter`

Attempt 2:

- 3 min: `ESLint 10.7.0 crashes on Node 18: TypeError: util.styleText is not a function`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
