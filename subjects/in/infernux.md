# Infernux

**Verdict: runs with mocks.** Argusic Score 56 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ChenlizheMe/Infernux, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/infernux

## Pinned environment

- Project commit: `d0eac0f2d29c0e606288e5f2d64b5b2fd30ae203`
- Test commit: `d0eac0f2d29c0e606288e5f2d64b5b2fd30ae203`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 15.9 to 25.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 15.9 | 0 | 0 | [run](https://argusic.com/run/2d301366-b83c-473e-8aa2-b75a04ad4a2b) |
| 2 | pass with mocks | 92 | 28 | 25.1 | 3 | 3 | [run](https://argusic.com/run/95271e47-ed6e-471d-9c4c-2f62f062df6f) |

## What was observed on a clean machine

Attempt 2:

- `Native C++ compiled extension (_Infernux.so) could not be built: missing system packages (no root access)`
- 3 min: `Python 3.13 required, system has Python 3.12`
- `CLI entry point (inx) and 279 native python/test tests unavailable without compiled native module`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
