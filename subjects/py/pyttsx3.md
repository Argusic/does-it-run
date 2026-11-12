# pyttsx3

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/nateshmbhat/pyttsx3, licensed MPL-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/pyttsx3

## Pinned environment

- Project commit: `8164fba9766293cfeef64145bc8d458a032f80fc`
- Test commit: `8164fba9766293cfeef64145bc8d458a032f80fc`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 4.1 to 5.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 20 | 4.1 | 2 | 2 | [run](https://argusic.com/run/200b112d-2798-4eca-8900-3ea596b814b9) |
| 2 | pass | 100 | 9 | 5.2 | 3 | 3 | [run](https://argusic.com/run/d2a36ff7-efa8-4611-8d9a-eea8d279d594) |

## What was observed on a clean machine

Attempt 1:

- 16 min: `RuntimeError: eSpeak or eSpeak-ng not installed , pyttsx3's _espeak.py ctypes loader could not find a libespeak-ng shared library`
- 1 min: `test_espeak_voices assertion failed: expected 131/141/221 voices but got 151 (newer espeak-ng data set)`

Attempt 2:

- 4 min: `espeak-ng shared library (libespeak-ng.so.1) not installed in the container`
- 4 min: `espeak-ng-data not found by the library at runtime (compiled-in path /usr/lib/x86_64-linux-gnu/espeak/espeak-ng-data doesn't exist)`
- 1 min: `Python package install failed due to externally managed environment (PEP 668)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
