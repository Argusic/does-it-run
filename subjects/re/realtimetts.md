# RealtimeTTS

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/KoljaB/RealtimeTTS, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/realtimetts

## Pinned environment

- Project commit: `50abd79cfb6033fe2781abc7c97291fe70dcc3ea`
- Test commit: `50abd79cfb6033fe2781abc7c97291fe70dcc3ea`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 13 to 13 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12.4 | 13 | 5 | 5 | [run](https://argusic.com/run/1aba2784-6116-4266-a203-04c7b71937bc) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `PyAudio failed to build: missing python3-dev and portaudio19-dev headers (no root access)`
- 1 min: `realtimetts[system] install failed because pyaudio build dependency failed`
- `ssh-keygen not available - release guard CLI attestation test fails`
- `SystemEngine pyttsx3 requires espeak/espeak-ng (no system TTS in container)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
