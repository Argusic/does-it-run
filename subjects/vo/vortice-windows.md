# Vortice.Windows

**Verdict: could not verify.** Argusic Score 32.5 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/amerkoleci/Vortice.Windows, licensed MIT, written in C.

Evidence and recordings: https://argusic.com/subject/vortice-windows

## Pinned environment

- Project commit: `4a799b871456155c23133e239e127c9fd23ac3c5`
- Test commit: `4a799b871456155c23133e239e127c9fd23ac3c5`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 2; wall time 18.5 to 21.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 50 | 7 | 18.5 | 1 | 1 | [run](https://argusic.com/run/caf9db28-632a-4062-b3d1-e927cd821ccb) |
| 2 | fail | 15 | 18 | 21.4 | 4 | 3 | [run](https://argusic.com/run/0b5cfdda-83c0-47ea-8fe3-f67759497df7) |

## What was observed on a clean machine

Attempt 1:

- 10 min: `SharpGenTools SDK requires Windows Registry to find Windows SDK C headers (SG0007 error)`

Attempt 2:

- 4 min: `dotnet SDK not installed in container`
- 2 min: `NETSDK1100: building Windows-targeted TFM on Linux`
- 6 min: `SharpGenTask not given CastXmlExecutable on Linux (SharpGen only bundles Windows castxml.exe)`
- 6 min: `SharpGen Windows SDK header resolution fails off-Windows: 'Unable to resolve registry paths when not on Windows', 'winerror.h' not found, SharpGen.Runtime.COM.h missing`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
