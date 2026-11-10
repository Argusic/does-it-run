# py-xiaozhi

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/huangjunsen0406/py-xiaozhi, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/py-xiaozhi

## Pinned environment

- Project commit: `9bfc807d368cccac71af8d9f7042ab6b5af92030`
- Test commit: `9bfc807d368cccac71af8d9f7042ab6b5af92030`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 4.2 to 16 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 3 | 16 | 6 | 6 | [run](https://argusic.com/run/0d3113c6-0ff0-44a1-b872-23b4e200e63f) |
| 2 | pass | 100 | 6 | 4.2 | 4 | 4 | [run](https://argusic.com/run/8f450794-571e-40c2-8c1e-b0404b0860a3) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `pip install failed with 'externally-managed-environment' (PEP 668)`
- 1 min: `evdev wheel build failed: fatal error: Python.h: No such file or directory (python3-dev missing from container)`
- 1 min: `pynput requires evdev which fails to build from source`
- 1 min: `PortAudio library not found by sounddevice at import`
- 1 min: `PySide6 missing for GUI-related test imports`
- 1 min: `hatchling missing at editable-install metadata generation`

Attempt 2:

- 3 min: `PortAudio library not found - sounddevice requires libportaudio2 at import time, but the system package is not installed and apt-get requires root`
- 0.5 min: `3 GUI tests failed due to PySide6 not being installed (base uv sync only)`
- 1 min: `Qt XCB platform plugin failed (libxcb-cursor0 missing, no root to install it)`
- 0.5 min: `Tests crashed with SIGABRT when Qt tried to initialize xcb platform without libxcb-cursor0`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
