# TheWhisper

**Verdict: runs with mocks.** Argusic Score 86.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/TheStageAI/TheWhisper, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/thewhisper

## Pinned environment

- Project commit: `af7eebaa53154d7d1edd545274e4a2df5a855ace`
- Test commit: `af7eebaa53154d7d1edd545274e4a2df5a855ace`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 34.5 to 34.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 86.29 | 35 | 34.5 | 7 | 5 | [run](https://argusic.com/run/4448873d-62e4-483a-84ea-09f40ccd6b23) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `ModuleNotFoundError: transformers on import thestage_speechkit`
- 5 min: `OSError: PortAudio library not found (system has no libportaudio.so, no root to install)`
- 3 min: `FileStream used librosa correctly but had typo orgi_sr and imported load unnecessarily`
- 20 min: `VAD streaming path silently dropped pending audio, and oversized queued chunks grew the buffer without trimming`
- 8 min: `Electron .env loaded from repo root but README runs from electron_app dir`
- 4 min: `Electron getUserMedia audio init returned {} in container (no audio device)`
- 2 min: `MLX/CoreML (apple) platform requires macOS; default server mode returns 500 on Linux`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
