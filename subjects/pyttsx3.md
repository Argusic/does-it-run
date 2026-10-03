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
- Valid runs: 1; wall time 4.1 to 4.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 20 | 4.1 | 2 | 2 | [run](https://argusic.com/run/200b112d-2798-4eca-8900-3ea596b814b9) |

## What was observed on a clean machine

Attempt 1:

- 16 min: `RuntimeError: eSpeak or eSpeak-ng not installed , pyttsx3's _espeak.py ctypes loader could not find a libespeak-ng shared library`
- 1 min: `test_espeak_voices assertion failed: expected 131/141/221 voices but got 151 (newer espeak-ng data set)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
