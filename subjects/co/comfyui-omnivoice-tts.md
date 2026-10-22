# ComfyUI-OmniVoice-TTS

**Verdict: runs.** Argusic Score 90 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Saganaki22/ComfyUI-OmniVoice-TTS, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/comfyui-omnivoice-tts

## Pinned environment

- Project commit: `3fe8e42a6d4a03628471aa1ba8506657e2e96dea`
- Test commit: `3fe8e42a6d4a03628471aa1ba8506657e2e96dea`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 4.9 to 14.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 6 | 14.2 | 3 | 3 | [run](https://argusic.com/run/e5424003-5c97-4829-a868-6742f6557f28) |
| 2 | pass | 100 | 5 | 4.9 | 7 | 7 | [run](https://argusic.com/run/d9b3f42a-c9b0-46af-bfef-2cd4ccfdce51) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `soundfile requires cffi/_cffi_backend`
- 1 min: `torchvision nms operator not found due to version mismatch`
- 1 min: `ComfyUI crashes on CUDA assertion at import with CPU-only PyTorch`

Attempt 2:

- 1.5 min: `No Python package manager found (externally managed environment); created venv`
- 1.5 min: `No module named 'torch'`
- 0.3 min: `No module named 'numpy'`
- 0.5 min: `No module named 'transformers'`
- 0.3 min: `No module named '_cffi_backend' (soundfile dep)`
- 0.3 min: `No module named 'accelerate' (needed by transformers from_pretrained)`
- 0.1 min: `OmniVoiceGenerationConfig arg 'steps' should be 'num_step'`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
