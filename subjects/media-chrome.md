# media-chrome

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/muxinc/media-chrome, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/media-chrome

## Pinned environment

- Project commit: `803787e819177c33f80a7b354f35e532b2215aca`
- Test commit: `803787e819177c33f80a7b354f35e532b2215aca`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 11 to 11 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2.5 | 11 | 3 | 3 | [run](https://argusic.com/run/dfafa2de-02fc-4e5e-964d-85e11d29479b) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `CHROME_PATH not set and no Chrome binary found`
- 1 min: `Chromium sandbox not available in container`
- 5 min: `5-6 tests fail: headless Chromium cannot decode H.264 video`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
