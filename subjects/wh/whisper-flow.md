# whisper-flow

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/dimastatz/whisper-flow, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/whisper-flow

## Pinned environment

- Project commit: `45855d46aa51ce0bde8eef82e17ef9142623daaa`
- Test commit: `45855d46aa51ce0bde8eef82e17ef9142623daaa`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 18 to 18 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 15 | 18 | 2 | 2 | [run](https://argusic.com/run/42930b5f-1d19-4704-9292-f709576d97e0) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `PyAudio==0.2.14 cannot build from source: C header Python.h is missing (python3-dev package not available without root). No pre-built wheel exists for this platform.`
- 1 min: `Coverage 94% < required 95% because whisperflow/audio/microphone.py is uncovered (hardware-dependent, excluded from CI via --ignore=tests/audio).`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
