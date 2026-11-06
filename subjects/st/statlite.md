# statlite

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/PVRLabs/statlite, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/statlite

## Pinned environment

- Project commit: `d13f3cb203c1019b6dec2eb0a34bfecf01a9b9c8`
- Test commit: `d13f3cb203c1019b6dec2eb0a34bfecf01a9b9c8`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 5 to 5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3.8 | 5 | 1 | 1 | [run](https://argusic.com/run/dbb07553-82d5-45ea-a856-be157a42dab7) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `go binary not installed in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
