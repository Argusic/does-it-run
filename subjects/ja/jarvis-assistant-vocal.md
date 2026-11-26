# jarvis-assistant-vocal

**Verdict: runs with mocks.** Argusic Score 86 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/sosoj92/jarvis-assistant-vocal, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/jarvis-assistant-vocal

## Pinned environment

- Project commit: `32faa786155a010d1a8a3ef47f95be46871d76ec`
- Test commit: `32faa786155a010d1a8a3ef47f95be46871d76ec`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, no run possible
- Valid runs: 2; wall time 6 to 35.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 1 | 35.7 | 6 | 6 | [run](https://argusic.com/run/5e385118-3a19-4c87-addf-60a9a32ae04b) |
| 2 | fail | 80 | 15 | 6 | 5 | 5 | [run](https://argusic.com/run/cb459c1f-3530-43da-a11c-197f1a6733f8) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `ctypes.windll import crashed tools.souris on Linux`
- 5 min: `os.startfile missing on Linux in tools/spotify.py and tools/systeme.py`
- 20 min: `sounddevice failed: PortAudio library not found; satellite module unittest couldn't import`
- 5 min: `Playwright Chromium missing (playwright install)`
- 25 min: `Signal Matin compact page overflow (content 1009px vs 975px), project PDF guard rejected page 3`
- 5 min: `4 unittest errors patching Windows-only os.startfile on Linux`

Attempt 2:

- 4 min: `ImportError: ctypes.windll.user32 on Linux in tools/souris.py blocked test_astra_pc and test_gestes_actions imports`
- 5 min: `AttributeError: os.startfile does not exist on Linux in test_web_routing and test_media_routing`
- 2 min: `OSError: PortAudio library not found for satellite_pi/jarvis_satellite import`
- 2 min: `RuntimeError: Chromium not installed for Playwright PDF tests`
- `AssertionError: test_no_major_overflow (compact mode) - page 3 overflows by 34px`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
