# RealtimeSTT

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/KoljaB/RealtimeSTT, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/realtimestt

## Pinned environment

- Project commit: `777727553eedfa19aead15337ce66bab549add3f`
- Test commit: `777727553eedfa19aead15337ce66bab549add3f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 7.9 to 8.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 25 | 7.9 | 1 | 1 | [run](https://argusic.com/run/c026217f-b5f2-4358-98f6-2eb2ed616795) |
| 2 | pass | 100 | 23 | 8.8 | 3 | 3 | [run](https://argusic.com/run/899d5a5f-e938-4d6b-b0b5-813e1f856795) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `PyAudio 0.2.14 source build failed because python3-dev and portaudio19-dev are not installed (no root privileges to apt-get install)`

Attempt 2:

- 9 min: `PyAudio==0.2.14 has no Linux wheel; build failed: PortAudio headers (portaudio.h) missing in container`
- 4 min: `PyAudio build failed again: Python.h not found (python3-dev headers missing)`
- 4 min: `Runtime ImportError: libportaudio.so.2 not found by pyaudio extension`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
