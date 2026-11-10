# elevenlabs-python

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/elevenlabs/elevenlabs-python, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/elevenlabs-python

## Pinned environment

- Project commit: `39d7bc9d02023f7a19a7356711832a47facf3aa4`
- Test commit: `39d7bc9d02023f7a19a7356711832a47facf3aa4`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 3.1 to 15.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 9 | 15.2 | 4 | 4 | [run](https://argusic.com/run/4cf7048d-f995-432a-b42f-eeed28b8995a) |
| 2 | pass with mocks | 92 | 0.32 | 3.1 | 2 | 2 | [run](https://argusic.com/run/7f0d29ac-17c8-450d-bee4-9a84a1deff63) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `pip install failed: externally-managed-environment`
- 3 min: `16 tests failed with 401 auth errors to real ElevenLabs API`
- 2 min: `test_tts_convert_with_timestamps: audio_base_64 was None`
- 2 min: `test_get_voice/test_get_voices failed on mock data`

Attempt 2:

- 0.1 min: `pyaudio optional dependency fails to build: missing Python.h (python3-dev headers not installed, no root access)`
- `16 tests fail with 401 authentication errors , they hit the live ElevenLabs API which requires an API key not provided in this environment`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
