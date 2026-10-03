# LEANN

**Verdict: runs with mocks.** Argusic Score 89.5 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/StarTrail-org/LEANN, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/leann

## Pinned environment

- Project commit: `f84dec41db5b0b7026a1f8dd18baafa55aa3d4a7`
- Test commit: `f84dec41db5b0b7026a1f8dd18baafa55aa3d4a7`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 86.8 to 86.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 89.5 | 85 | 86.8 | 8 | 7 | [run](https://argusic.com/run/62ac26cb-addf-401a-823a-9c49ece21739) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `uv not found, needed for Python package management`
- 3 min: `Git submodules not initialized`
- 3 min: `pkg-config could not find libzmq (only libzmq5 runtime was installed, no .pc file)`
- 5 min: `CMake FindBLAS could not find BLAS (only libblas3 runtime, no .so symlink without version)`
- 5 min: `CMake could not find SWIG during Faiss build`
- 5 min: `Faiss SWIG module compiled with numpy 1.x but env had numpy 2.x, causing SystemError at import`
- 10 min: `Faiss Python wrapper files had circular import structure when nested under leann_backend_hnsw`
- 10 min: `leann-backend-diskann requires libaio and Boost system packages (no root access)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
