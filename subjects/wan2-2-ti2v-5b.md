# Wan2.2-TI2V-5B

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://huggingface.co/Wan-AI/Wan2.2-TI2V-5B, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/wan2-2-ti2v-5b

## Pinned environment

- Project commit: `921dbaf3f1674a56f47e83fb80a34bac8a8f203e`
- Test commit: `921dbaf3f1674a56f47e83fb80a34bac8a8f203e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: gpu
- Test depth: real run
- Valid runs: 2; wall time 29.7 to 64.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 10 | 29.7 | 7 | 7 | [run](https://argusic.com/run/11528610-c7d1-4df3-9b9f-65cae61c4ac1) |
| 1 | pass | 100 | 63 | 64.9 | 4 | 4 | [run](https://argusic.com/run/5ff50baf-abdf-41cb-800c-a7945fc35dcd) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `pip install blocked by externally-managed-environment on Debian`
- 5 min: `flash-attn failed to build from source: missing packaging, CUDA_HOME, torch not found, PEP 517 build issues, setuptools/packaging conflicts, missing Python.h, C++20 requirement for torch 2.14`
- 2 min: `torch 2.14+cu130 requires CUDA driver >= 12.80 but driver 570.195.03 reports CUDA 12.8 compatibility`
- 2 min: `Missing Python dependencies: einops, decord, librosa, peft (triggered by eager imports in wan/__init__.py of unused S2V and Animate modules)`
- 1 min: `numpy version conflict: Wan requires numpy<2 but librosa, scipy, opencv-python, transformers require numpy>=2`
- 0.5 min: `AssertionError in flash_attention when flash_attn not installed (flash_attention() called directly by WanSelfAttention with assert FLASH_ATTN_2_AVAILABLE)`
- 0.3 min: `Shape mismatch in SDPA fallback (returned [B*L, N, C] instead of [B, L, N, C])`

Attempt 1:

- 15 min: `flash-attn cannot compile without CUDA_HOME/nvcc`
- 8 min: `CUDA OOM at 121 frames (VAE decode)`
- 3 min: `Missing packages: einops, decord, librosa, peft, packaging`
- 2 min: `librosa 1.0.0 incompatible with numpy<2`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
