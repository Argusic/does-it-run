# lnxlink

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/bkbilly/lnxlink, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/lnxlink

## Pinned environment

- Project commit: `870847c235d4615881f39c852adbbfc72a2bfa7c`
- Test commit: `870847c235d4615881f39c852adbbfc72a2bfa7c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 6.9 to 6.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 18 | 6.9 | 3 | 3 | [run](https://argusic.com/run/1ead04c9-e02e-473b-9327-4c3e71aed0e7) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `No D-Bus daemon in container: jeepney open_dbus_connection FileNotFoundError (system_monitor.py)`
- 4 min: `Environment modules active_window/clipboard/current_user/night_light/bluetooth/dnd failed to init in headless container (no X session/loginctl/backends)`
- 6 min: `README install path pipx not available; system Python is PEP 668 externally-managed`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
