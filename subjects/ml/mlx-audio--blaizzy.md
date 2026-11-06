# mlx-audio

**Verdict: runs with mocks.** Argusic Score 82.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Blaizzy/mlx-audio, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/run/f3da1484-bf49-4b16-8d52-452be46ab0e4

## Pinned environment

- Project commit: `4ab7e6f7dedd69a136cfaa318c5dc8aed5119446`
- Test commit: `4ab7e6f7dedd69a136cfaa318c5dc8aed5119446`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, no run possible
- Valid runs: 2; wall time 8.2 to 11.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 7.5 | 8.2 | 4 | 4 | [run](https://argusic.com/run/f3da1484-bf49-4b16-8d52-452be46ab0e4) |
| 2 | fail | 73.33 | 5 | 11.1 | 3 | 2 | [run](https://argusic.com/run/bf7aba0d-7b9b-46ec-b6ee-cd8a302c54f2) |

## What was observed on a clean machine

Attempt 1:

- 1.5 min: `mlx.core imported libmlx.so but libmlx.so was not bundled with the base pip install on Linux (Apple Silicon-only by default)`
- 1 min: `pip install failed due to externally-managed-environment (PEP 668)`
- 1 min: `webrtcvad failed to build from source (needs Python.h / python3-dev, not available)`
- 1.5 min: `sounddevice requires PortAudio runtime library (libportaudio2 not available)`

Attempt 2:

- 1 min: `webrtcvad cannot build: missing Python.h (python3-dev not installed, no root)`
- 1 min: `mlx wheel missing libmlx.so on Linux; mlx[cpu] extra required`
- 2 min: `TTS --help crashed at module level because audio_player imports portaudio-dependent sounddevice`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
