# ComfyUI-VoxCPM

**Verdict: runs with mocks.** Argusic Score 56 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/wildminder/ComfyUI-VoxCPM, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/comfyui-voxcpm

## Pinned environment

- Project commit: `2d1e32ec7d69cf2d002b0480c6113c0b68e0baef`
- Test commit: `2d1e32ec7d69cf2d002b0480c6113c0b68e0baef`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 3.8 to 8.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 3.8 | 0 | 0 | [run](https://argusic.com/run/b2b35f6e-6eae-428b-9137-0979669170bc) |
| 2 | pass with mocks | 92 | 28 | 8.7 | 3 | 3 | [run](https://argusic.com/run/82250abe-e372-4ed9-aa1d-1eae00a2b7fb) |

## What was observed on a clean machine

Attempt 2:

- 8 min: `ComfyUI model_management.py crashes on CPU-only systems via torch.cuda.current_device() at module level`
- 5 min: `conftest.py had hardcoded Windows dev path for COMFYUI_ROOT`
- 3 min: `test_dataset_utils.py imported nonexistent functions (estimate_audio_duration, validate_audio_duration, format_duration)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
