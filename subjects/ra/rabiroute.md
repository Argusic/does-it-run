# RabiRoute

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/vb2250158/RabiRoute, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/rabiroute

## Pinned environment

- Project commit: `366c9f5fed323879cd584bf57f694fca45fa9cc0`
- Test commit: `366c9f5fed323879cd584bf57f694fca45fa9cc0`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 44.9 to 44.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 4 | 44.9 | 10 | 10 | [run](https://argusic.com/run/23913fd4-10e5-46fc-9d64-e87c6dbd8733) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `System Node v18.19.1 did not satisfy the required >=22.13.0`
- 8 min: `Clean-state startup did not seed example data and /api/roles returned HTTP 500`
- 2 min: `Invalid .gitkeep inside the canonical plan archive directory failed plan-storage validation`
- 12 min: `Windows workspace path comparisons failed on Linux test hosts`
- 2 min: `Browser test assumed a browser executable was installed`
- 2 min: `PowerShell-dependent windows-desktop-contract test failed on Linux`
- 6 min: `Async timers were unreferenced and allowed awaited preparation or shutdown work to be abandoned`
- 2 min: `Developer verification script passed an invalid experimental test-isolation flag`
- 4 min: `Application shutdown converted a retirement timeout into an unconfirmed AggregateError`
- 1 min: `Post-shutdown host status read encountered a missing stale process-lease control file`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
