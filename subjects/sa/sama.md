# SAMA

**Verdict: not yet verified.** Argusic Score 50 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Cynthiazxy123/SAMA, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/sama

## Pinned environment

- Project commit: `85441d5d42e6335f66282b92016eae7266df436e`
- Test commit: `85441d5d42e6335f66282b92016eae7266df436e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 1; wall time 9.2 to 9.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 50 | 6 | 9.2 | 3 | 3 | [run](https://argusic.com/run/81dd47f6-c6ee-41dd-8ee4-8b4b2aaad0da) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `ModuleNotFoundError: No module named examples - inference.py imports from examples.wanvideo.model_training.custom_utils which is in repo but missing __init__.py files`
- 1 min: `ModuleNotFoundError: No module named pkg_resources - setuptools needed for setup.py build`
- 2 min: `Missing GPU-only packages: flash_attn, cupy-cuda12x, nvidia-* driver packages cannot install without CUDA hardware/libcuda`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
