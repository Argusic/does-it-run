# jietuba

**Verdict: runs with mocks.** Argusic Score 56 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/1003129155/jietuba, licensed MIT, written in C++.

Evidence and recordings: https://argusic.com/subject/jietuba

## Pinned environment

- Project commit: `2d720c9d16c6d6302c22b56c02a85ddd90defefb`
- Test commit: `2d720c9d16c6d6302c22b56c02a85ddd90defefb`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 8.2 to 59.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 8.2 | 0 | 0 | [run](https://argusic.com/run/e1c7dd3b-f5b0-4b5d-80a2-62c27077aaa9) |
| 2 | pass with mocks | 92 | 25 | 59.5 | 8 | 8 | [run](https://argusic.com/run/8d3582d4-b98f-4820-8c5a-f3624dd5d3d7) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `Python 3.11 required but container has 3.12`
- 3 min: `pywin32 (Windows-only) not available on Linux`
- 2 min: `comtypes (Windows-only) not available on Linux`
- 5 min: `ctypes.windll not available on Linux`
- 5 min: `gifrecorder Rust crate links Windows user32/gdi32, cannot build`
- 8 min: `evdev (pynput dependency) requires python3-dev headers for C compilation`
- 1 min: `winreg module not available on Linux`
- 1 min: `PyInstaller not pre-installed for test_build_script`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
