# totk-pc-recomp

**Verdict: runs with mocks.** Argusic Score 56 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/valentderah/totk-pc-recomp, licensed MIT, written in C.

Evidence and recordings: https://argusic.com/subject/totk-pc-recomp

## Pinned environment

- Project commit: `c38e0ca13d2bceb0590b195f69a010315913850d`
- Test commit: `c38e0ca13d2bceb0590b195f69a010315913850d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 31.5 to 48 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 47 | 48 | 5 | 5 | [run](https://argusic.com/run/767eaab5-cdb8-40dd-b529-19df11e9d88d) |
| 2 | fail | 20 | 30 | 31.5 | 6 | 6 | [run](https://argusic.com/run/61819a0c-163f-4ca3-946c-04cd1b917331) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Clang compiler not available in default environment`
- 1 min: `uv not found on PATH`
- 3 min: `spirv-val not available for shader validation`
- 2 min: `.NET SDK 10 not installed`
- 1 min: `excl_mt ABA test fails on CAS-based exclusive monitor emulation`

Attempt 2:

- 8 min: `No C compiler in container (clang/lld/ninja)`
- 1 min: `Python 3.14 not available for .venv-py314`
- 12 min: `Full totk.exe C build fails: Vulkan 1.3.275 from apt lacks VK_KHR_DYNAMIC_RENDERING_LOCAL_READ (needs 1.4+), SDL3 not in apt, clang 18 lacks C23 #embed`
- 2 min: `clang 18.1.3 from Ubuntu rejects __builtin_cpu_supports("sha") in sha256.c`
- `tests/excl_mt.py ABA test fails (cmpxchg limitation on x86)`
- `tests/worktree_test.py fails on Linux (Windows-style junctions)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
