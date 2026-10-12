# pytools

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/CharlesPikachu/pytools, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/pytools

## Pinned environment

- Project commit: `58eaf9dbd1bc93541abee16c7d86a69c4e052897`
- Test commit: `58eaf9dbd1bc93541abee16c7d86a69c4e052897`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 15 to 15 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 13 | 15 | 4 | 4 | [run](https://argusic.com/run/0123b15a-0ca3-42e7-8f7a-76725415cb57) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `tkinter module not available (system library missing, no root to install python3-tk)`
- 4 min: `js2py incompatible with Python 3.12 new bytecode (LOAD_ATTR flag-bit encoding, CACHE instructions, code.replace() API change)`
- 1.5 min: `libpulse-mainloop-glib.so.0 not found (PyQt5 QtMultimedia dependency)`
- 0.5 min: `Missing pip packages: pyttsx3, tqdm`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
