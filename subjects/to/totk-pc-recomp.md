# totk-pc-recomp

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/valentderah/totk-pc-recomp, licensed MIT, written in C.

Evidence and recordings: https://argusic.com/subject/totk-pc-recomp

## Pinned environment

- Project commit: `c38e0ca13d2bceb0590b195f69a010315913850d`
- Test commit: `c38e0ca13d2bceb0590b195f69a010315913850d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 48 to 48 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 47 | 48 | 5 | 5 | [run](https://argusic.com/run/767eaab5-cdb8-40dd-b529-19df11e9d88d) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Clang compiler not available in default environment`
- 1 min: `uv not found on PATH`
- 3 min: `spirv-val not available for shader validation`
- 2 min: `.NET SDK 10 not installed`
- 1 min: `excl_mt ABA test fails on CAS-based exclusive monitor emulation`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
