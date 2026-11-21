# VoiceStreamAI

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/alesaccoia/VoiceStreamAI, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/voicestreamai

## Pinned environment

- Project commit: `9248cd1fcf267b105f7d88b8d93e5b840009445e`
- Test commit: `9248cd1fcf267b105f7d88b8d93e5b840009445e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 15.4 to 41.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 15.4 | 3 | 3 | [run](https://argusic.com/run/031ccbab-e424-4816-829d-93a7a770a7e8) |
| 2 | pass | 100 | 35 | 41.6 | 3 | 3 | [run](https://argusic.com/run/93542bf9-f7bf-48e4-a114-e5b64f1b66a0) |

## What was observed on a clean machine

Attempt 1:

- 22 min: `faster-whisper's download_model rejects local paths (HFValidationError: Repo id must be in the form 'repo_name' or 'namespace/repo_name'), so a local stand-in ASR model cannot be pointed at directly`
- 8 min: `server buffering logic with --vad-type none sent no transcription when the full audio payload was streamed without a trailing silence offset (first three server runs produced 0 replies, logged ConnectionClosed with code 1000 OK)`
- 8 min: `test/vad/test_pyannote_vad.py setUp fails: PyannoteVAD() without auth raises 'Missing required env var in PYANNOTE_AUTH_TOKEN'; the pyannote/segmentation model is access-restricted (huggingface.co returned HTTP 401)`

Attempt 2:

- 10 min: `test/server/test_server.py default VAD_TYPE=pyannote requires HF auth token, missing event loop with websockets 12.x`
- 3 min: `test/asr/test_asr.py default ASR_TYPE=whisper (HF pipeline) removed, no model args configurable`
- 5 min: `test/vad/test_pyannote_vad.py always requires PYANNOTE_AUTH_TOKEN for gated pyannote/segmentation model`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
