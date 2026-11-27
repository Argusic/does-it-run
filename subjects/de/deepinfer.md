# DeepInfer

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/deepseek-ai/DeepInfer, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/deepinfer

## Pinned environment

- Project commit: `9bd9cf243fc53ef9afbf8f04d391d989117d6ab9`
- Test commit: `9bd9cf243fc53ef9afbf8f04d391d989117d6ab9`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 30.7 to 30.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 12 | 30.7 | 3 | 3 | [run](https://argusic.com/run/f1ca96dc-254d-43a0-88a3-72f564af8fff) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `C extension (deepinfer._C) cannot be compiled: nvcc not available, CUDA_HOME not found in container`
- 2 min: `tile_kernels pip package hangs at import (CUDA init)`
- 3 min: `Vendor submodules (DeepEP, FlashMLA, DeepSelect, DeepGEMM) empty, cannot build without CUDA`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
