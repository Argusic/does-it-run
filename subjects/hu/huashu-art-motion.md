# huashu-art-motion

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/alchaincyf/huashu-art-motion, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/huashu-art-motion

## Pinned environment

- Project commit: `9ff59339f934e08483ba0a5b1db20f4c2c421b35`
- Test commit: `9ff59339f934e08483ba0a5b1db20f4c2c421b35`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 15 to 15 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 15 | 15 | 3 | 3 | [run](https://argusic.com/run/f8620401-51ec-4cd4-b42a-a8dabfc5322a) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `uv not pre-installed in container`
- 4 min: `Playwright Chromium browser not installed`
- 3 min: `Python dependencies missing for test suite (requests, Pillow, numpy, opencv-python-headless)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
