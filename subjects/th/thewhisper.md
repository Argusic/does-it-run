# TheWhisper

**Verdict: runs.** Argusic Score 93.1 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/TheStageAI/TheWhisper, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/thewhisper

## Pinned environment

- Project commit: `af7eebaa53154d7d1edd545274e4a2df5a855ace`
- Test commit: `af7eebaa53154d7d1edd545274e4a2df5a855ace`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 11.9 to 34.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 86.29 | 35 | 34.5 | 7 | 5 | [run](https://argusic.com/run/4448873d-62e4-483a-84ea-09f40ccd6b23) |
| 2 | pass | 100 | 2 | 11.9 | 6 | 6 | [run](https://argusic.com/run/b5245c1c-b39a-474f-9fa8-9ae0ba9f3fdb) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `ModuleNotFoundError: transformers on import thestage_speechkit`
- 5 min: `OSError: PortAudio library not found (system has no libportaudio.so, no root to install)`
- 3 min: `FileStream used librosa correctly but had typo orgi_sr and imported load unnecessarily`
- 20 min: `VAD streaming path silently dropped pending audio, and oversized queued chunks grew the buffer without trimming`
- 8 min: `Electron .env loaded from repo root but README runs from electron_app dir`
- 4 min: `Electron getUserMedia audio init returned {} in container (no audio device)`
- 2 min: `MLX/CoreML (apple) platform requires macOS; default server mode returns 500 on Linux`

Attempt 2:

- 0.5 min: `pip install .[nvidia] fails: nvidia-cuda-runtime-cu13 wheel build error (no CUDA toolchain)`
- 0.2 min: `sounddevice import fails: PortAudio library not found`
- 0.1 min: `thestage_speechkit.apple import fails: mlx not installed`
- 0.1 min: `benchmark/eval_utils.py fails: ModuleNotFoundError for whisper_normalizer`
- 0.1 min: `Electron binary can't run: SUID sandbox helper not configured`
- `examples/server.py add_chunk endpoint uses query param for base64 audio data, hits URL size limit for real audio`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
