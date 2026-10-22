# B

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/AhmadHassan-BTed/B, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/b

## Pinned environment

- Project commit: `d34943d3ea89a9dbf2d0104e5ccf31c5696d35f4`
- Test commit: `d34943d3ea89a9dbf2d0104e5ccf31c5696d35f4`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 28.4 to 28.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 23 | 28.4 | 8 | 8 | [run](https://argusic.com/run/10b66630-1ad4-4a89-8f46-a6f92654b534) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Module 'groq' not found`
- 3 min: `uiautomation import fails on Linux (COM only on Windows)`
- 2 min: `No module 'torch' for audio/ears.py`
- 3 min: `PortAudio library not found (sounddevice)`
- 5 min: `ctypes.windll not available on Linux`
- 2 min: `auto.uiautomation.SetGlobalSearchTimeout missing`
- 1 min: `winocr has no recognize_pil`
- 2 min: `OCR result has no .lines attribute`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
