# color

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/gookit/color, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/color

## Pinned environment

- Project commit: `9bc305ff3e85a83ab29d3abf7ee659dbb5fcaf1a`
- Test commit: `9bc305ff3e85a83ab29d3abf7ee659dbb5fcaf1a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 11 to 11 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 10 | 11 | 2 | 2 | [run](https://argusic.com/run/3f2f4997-b713-4df7-81ad-1fdfdd68938f) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `Go compiler not found in container (Ubuntu 24.04, no root access)`
- 2 min: `All color rendering tests failed with 'actual: msg' instead of ANSI escape codes because NO_COLOR=1 set Enable=false at package init`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
