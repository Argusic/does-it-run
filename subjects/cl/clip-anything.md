# Clip-Anything

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/SamurAIGPT/Clip-Anything, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/clip-anything

## Pinned environment

- Project commit: `f455b2d306cec77d05b0060c34fa0112f1802a10`
- Test commit: `f455b2d306cec77d05b0060c34fa0112f1802a10`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 7.5 to 7.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 7.4 | 7.5 | 6 | 6 | [run](https://argusic.com/run/754ec920-1fe2-4b35-a17c-a6dd0b80e529) |

## What was observed on a clean machine

Attempt 1:

- 0.1 min: `python command not found (Debian uses python3)`
- 0.2 min: `Externally-managed pip environment blocks system install`
- 1 min: `moviepy 2.x removed moviepy.editor module`
- 0.3 min: `ffmpeg prompts for overwrite on temp_audio.wav`
- 1 min: `Hardcoded 'Bearer groq-key' and groq.com URL in app.py`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
