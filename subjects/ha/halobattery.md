# HaloBattery

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/HeyOkay/HaloBattery, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/halobattery

## Pinned environment

- Project commit: `73e229cbee2e97fad659fcd96c78afdfa78488fb`
- Test commit: `73e229cbee2e97fad659fcd96c78afdfa78488fb`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 6 to 18.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 18 | 18.9 | 3 | 3 | [run](https://argusic.com/run/960c9a43-4fc7-4a51-92a5-19543cf5a93c) |
| 2 | pass with mocks | 92 | 6 | 6 | 2 | 2 | [run](https://argusic.com/run/b8d9b8a9-b0e9-4680-9b4a-4c921c261af6) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Python import system on Linux does not recognize .pyw as a source suffix, so spec_from_file_location() returned None for halo_battery.pyw in 6 test files, cascading into ~34 import errors`
- 5 min: `_sandbox.install_guards() replaced socket.socket.connect to block ALL connections including local Unix domain sockets used by X11, causing pystray's Xorg backend import to fail`
- 1 min: `3 test_startup_imports subprocess tests failed because the child process also hit the X11 sandbox guard via pystray import`

Attempt 2:

- 3 min: `importlib.util.spec_from_file_location returns None for .pyw files on Linux`
- 5 min: `pystray X11 backend connects to /tmp/.X11-unix/X99 during import, blocked by sandbox no-network guard`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
