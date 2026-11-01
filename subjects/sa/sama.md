# SAMA

**Verdict: runs with mocks.** Argusic Score 71 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Cynthiazxy123/SAMA, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/sama

## Pinned environment

- Project commit: `85441d5d42e6335f66282b92016eae7266df436e`
- Test commit: `85441d5d42e6335f66282b92016eae7266df436e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 9.2 to 12.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 50 | 6 | 9.2 | 3 | 3 | [run](https://argusic.com/run/81dd47f6-c6ee-41dd-8ee4-8b4b2aaad0da) |
| 2 | pass with mocks | 92 | 12 | 12.3 | 5 | 5 | [run](https://argusic.com/run/4dd5e131-0c35-4fdf-97e1-f6124b20b9cc) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `ModuleNotFoundError: No module named examples - inference.py imports from examples.wanvideo.model_training.custom_utils which is in repo but missing __init__.py files`
- 1 min: `ModuleNotFoundError: No module named pkg_resources - setuptools needed for setup.py build`
- 2 min: `Missing GPU-only packages: flash_attn, cupy-cuda12x, nvidia-* driver packages cannot install without CUDA hardware/libcuda`

Attempt 2:

- 2 min: `flash_attn build failed: CUDA_HOME/nvcc not found`
- 1 min: `deepspeed build failed: CUDA_HOME/nvcc not found`
- 1 min: `cupy-cuda12x build failed: CUDA not available`
- 2 min: `pip diffsynth v2.2.0 vs local v1.1.8 version conflict`
- 1 min: `examples/ module not on sys.path`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
