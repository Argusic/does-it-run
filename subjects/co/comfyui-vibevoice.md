# ComfyUI-VibeVoice

**Verdict: runs with mocks.** Argusic Score 81 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/wildminder/ComfyUI-VibeVoice, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/comfyui-vibevoice

## Pinned environment

- Project commit: `774c1aeeb374bdb6312f68be1be3ad9e781ed557`
- Test commit: `774c1aeeb374bdb6312f68be1be3ad9e781ed557`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 30 to 31 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 70 | 1.5 | 30 | 2 | 1 | [run](https://argusic.com/run/8b2b325b-6c63-4397-980b-34423bac490c) |
| 2 | pass with mocks | 92 | 11 | 31 | 4 | 4 | [run](https://argusic.com/run/8d59ff1c-39ee-4a20-846d-1c56707df824) |

## What was observed on a clean machine

Attempt 1:

- `ComfyUI core not installed; ComfyUI stubs created for test isolation (comfy_api.latest, comfy.model_management, comfy.utils, folders_paths, etc.)`
- `1515/1639 tests pass; 87 fail + 5 errors in streaming quant load, cache compat, fp8 resident detection, and prompt validation paths requiring full ComfyUI core or comfy_kitchen dequant kernels`

Attempt 2:

- 8 min: `Missing ComfyUI dependencies (comfy.model_management, comfy.utils, comfy.model_patcher, comfy.ops, comfy_kitchen, comfy_api.latest)`
- 2 min: `io.Schema/io.NodeOutput/Custom type stubs incomplete`
- 1 min: `gguf module not installed`
- `230 tests still failing: require full ComfyUI installation, real model weights from HuggingFace, or GPU`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
