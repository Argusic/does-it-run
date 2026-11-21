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
- Valid runs: 2; wall time 9.7 to 15 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 13 | 15 | 4 | 4 | [run](https://argusic.com/run/0123b15a-0ca3-42e7-8f7a-76725415cb57) |
| 2 | pass | 100 | 0.1 | 9.7 | 10 | 10 | [run](https://argusic.com/run/fb9162bb-e037-4438-93d5-41e25e6fd974) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `tkinter module not available (system library missing, no root to install python3-tk)`
- 4 min: `js2py incompatible with Python 3.12 new bytecode (LOAD_ATTR flag-bit encoding, CACHE instructions, code.replace() API change)`
- 1.5 min: `libpulse-mainloop-glib.so.0 not found (PyQt5 QtMultimedia dependency)`
- 0.5 min: `Missing pip packages: pyttsx3, tqdm`

Attempt 2:

- 0.1 min: `No python command (only python3)`
- 0.5 min: `pip externally-managed-environment error`
- 0.2 min: `Missing setuptools in venv`
- 2 min: `Missing tkinter system package (no root access)`
- 3 min: `modules/__init__.py eager imports cascade-failed on tkinter/turtle/js2py`
- 0.5 min: `pytools.py used 'from .modules import *' incompatible with lazy loading`
- 1 min: `js2py 0.74 injector broken on Python 3.12`
- 0.3 min: `Missing tqdm dependency`
- 0.3 min: `Missing pyttsx3 dependency`
- 0.5 min: `videoplayer/musicplayer need libpulse-mainloop-glib.so.0 system library`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
