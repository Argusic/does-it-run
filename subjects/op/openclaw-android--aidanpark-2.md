# openclaw-android

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/AidanPark/openclaw-android, licensed MIT, written in Kotlin.

Evidence and recordings: https://argusic.com/run/dbe0cc9c-1f96-4b05-b462-602826fb290c

## Pinned environment

- Project commit: `cfb0740fc0961f1dd1c2a22ecf133eae443fa96f`
- Test commit: `cfb0740fc0961f1dd1c2a22ecf133eae443fa96f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 4.6 to 4.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 3 | 4.6 | 2 | 2 | [run](https://argusic.com/run/dbe0cc9c-1f96-4b05-b462-602826fb290c) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `install.sh requires Termux ($PREFIX) which does not exist on standard Linux`
- 0.5 min: `verify-compat.sh: 6/15 failures on non-Termux (LD_PRELOAD lifecycle, glibc-compat.js, npm script-shell)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
