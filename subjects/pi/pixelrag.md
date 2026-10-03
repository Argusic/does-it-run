# PixelRAG

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/StarTrail-org/PixelRAG, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/pixelrag

## Pinned environment

- Project commit: `aba824b3172c58e7c76f5ee61a06dcec18c1c7cf`
- Test commit: `aba824b3172c58e7c76f5ee61a06dcec18c1c7cf`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 4 to 4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1 | 4 | 2 | 2 | [run](https://argusic.com/run/2bcaeee0-09fe-4d03-92e6-70aef273ffa3) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Missing pytest - dev extra not installed`
- 1 min: `Missing zstandard - Chrome headless_shell extraction fails`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
