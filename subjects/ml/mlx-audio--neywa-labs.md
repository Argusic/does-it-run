# mlx-audio

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Neywa-Labs/mlx-audio, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/run/d5935054-e9c1-42bd-9e02-42f1e3885be2

## Pinned environment

- Project commit: `e0833581c52963ff52b9916dc6eace8ca870aae0`
- Test commit: `e0833581c52963ff52b9916dc6eace8ca870aae0`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 9.9 to 39.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 38 | 39.2 | 13 | 13 | [run](https://argusic.com/run/d5935054-e9c1-42bd-9e02-42f1e3885be2) |
| 2 | pass | 100 | 9 | 9.9 | 5 | 5 | [run](https://argusic.com/run/dcd1d7ce-d951-4e42-acff-76118058f3ad) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `pip install -e '.[dev,server]' failed while building webrtcvad because Python.h was absent.`
- 2 min: `mlx==0.32.4 installed but importing mlx.core failed because libmlx.so was missing.`
- 4 min: `mlx_audio.tts.generate failed at import because sounddevice could not find PortAudio, even when --play was not requested.`
- 14 min: `The inference broker unconditionally created an MLX GPU stream; on the CPU-only Linux build the worker crashed and requests hung.`
- 1 min: `Optional-dependency tests failed with TypeError because a set was intersected with a list.`
- 2 min: `Optional-dependency resolve tests invoked system pip and failed under PEP 668.`
- 2 min: `GPU-only modelopt tests ran on the CPU-only MLX build and raised 'Cannot get gpu stream without gpu backend'.`
- 2 min: `Nemotron bfloat16 modelopt tests failed because CPU GatherMM supports only float32.`
- 8 min: `Kokoro generation failed after model load because misaki.en lacked num2words and spacy; the endpoint had already committed HTTP 200 and then closed with an empty body.`
- 5 min: `Qwen3-TTS routing tests fell through into native non-ICL generation and segfaulted on the CPU backend.`
- 3 min: `Spark TTS import failed because soxr was missing.`
- 2 min: `The Fish Drama3 decode-memory heuristic failed due to allocator bucket rounding.`
- 4 min: `PortAudio-dependent test collection failed because the native library was absent and system packages could not be installed.`

Attempt 2:

- 1 min: `PEP 668 externally-managed-environment blocked system pip install`
- 2 min: `webrtcvad build failed: Python.h not found, no root apt`
- 1 min: `sounddevice requires PortAudio system library, not packaged`
- 1 min: `mlx[cpu]==0.32.4 needed as separate package for Linux (mlx-core without GPU backend)`
- 1 min: `test_selective_scan GPU parametrize fails on CPU-only machine`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
