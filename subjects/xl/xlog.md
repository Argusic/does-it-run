# xlog

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/emad-elsaid/xlog, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/xlog

## Pinned environment

- Project commit: `f0e4d8d20168413cdcf6339384831fd6660d3702`
- Test commit: `f0e4d8d20168413cdcf6339384831fd6660d3702`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 29.5 to 29.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 30 | 29.5 | 2 | 2 | [run](https://argusic.com/run/6817e7b3-f05d-4ad2-b9ab-b117c0837db4) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Go 1.26 compiler not found in container`
- 5 min: `Go std library source missing (golang-1.26-src package was a transitional stub)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
