# zvec

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/alibaba/zvec, licensed Apache-2.0, written in C++.

Evidence and recordings: https://argusic.com/subject/zvec

## Pinned environment

- Project commit: `53c1bb60a0e560272db45eb53a4a596cbdecb2b8`
- Test commit: `53c1bb60a0e560272db45eb53a4a596cbdecb2b8`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 57.5 to 57.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 49.6 | 57.5 | 5 | 5 | [run](https://argusic.com/run/1b8788a6-0cbb-4ff5-bd9c-c9f2959186b3) |

## What was observed on a clean machine

Attempt 1:

- 2.5 min: `python3.12-dev headers not installed - CMake/pybind11 FindPythonLibsNew resolves INCLUDEPY to /usr/include/python3.12 which doesn't exist`
- 5.8 min: `pybind11::module INTERFACE_INCLUDE_DIRECTORIES hard-codes /usr/include/python3.12 from sysconfig; system cmake 3.28 vs pip cmake 3.31 behaves differently`
- 2.7 min: `Python.h includes <x86_64-linux-gnu/python3.12/pyconfig.h> which was not present`
- 7.3 min: `Parallel build of _zvec.so fails because static lib targets (core_knn_flat_static, etc.) are not built before linking`
- 0.5 min: `Pip-installed Python wrapper layer v0.7.0 mismatched freshly-built _zvec.so API (tuple vs _Doc objects)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
