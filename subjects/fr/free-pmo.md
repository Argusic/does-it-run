# free-pmo

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/nafiesl/free-pmo, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/free-pmo

## Pinned environment

- Project commit: `a8a0dd83e147d5bbd9f39a7dd337348bbecc194f`
- Test commit: `a8a0dd83e147d5bbd9f39a7dd337348bbecc194f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 7.8 to 7.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 7.8 | 2 | 2 | [run](https://argusic.com/run/2073728b-5304-43df-86a6-ce6022df2d31) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `PHP not installed in container`
- 1 min: `GD extension lacks JPEG support in static PHP binary causing 2 test failures`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
