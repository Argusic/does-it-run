# VibeVoice-ComfyUI

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Enemyx-net/VibeVoice-ComfyUI, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/vibevoice-comfyui

## Pinned environment

- Project commit: `b0a8efc23c9d902d7ebd8fe3f79515a23d343bc2`
- Test commit: `b0a8efc23c9d902d7ebd8fe3f79515a23d343bc2`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 7.6 to 21.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 0.12 | 21.9 | 0 | 0 | [run](https://argusic.com/run/d17e1bcf-54a0-43bf-a82b-84ce506f93a4) |
| 2 | pass with mocks | 92 | 5 | 7.6 | 2 | 2 | [run](https://argusic.com/run/1130017c-8f12-4b56-90e0-d60773085a14) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `pip install -e . fails: pyproject.toml has flat-layout conflict with 'nodes' and 'vvembed' top-level packages`
- `bitsandbytes warns: 'Failed to load CPU gemm_4bit_forward from kernels-community: No module named kernels'`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
