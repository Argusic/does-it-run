# f-flow

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Foblex/f-flow, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/f-flow

## Pinned environment

- Project commit: `3b7e93fb14ebfb53b2d84a48f5b12d133dd3dbfe`
- Test commit: `3b7e93fb14ebfb53b2d84a48f5b12d133dd3dbfe`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 12.7 to 12.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 12.7 | 2 | 2 | [run](https://argusic.com/run/2adb661f-d620-4c13-8226-fc99b8b48394) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Node.js v18.19.1 too old for Angular CLI (needs v20.19+)`
- 1 min: `Chrome crashes with 'No usable sandbox' on Ubuntu 24.04`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
