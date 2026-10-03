# listen1_desktop

**Verdict: could not verify.** Argusic Score 80 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/listen1/listen1_desktop, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/listen1-desktop

## Pinned environment

- Project commit: `bbc38654bd593d4ae70143230ea7814b34d09128`
- Test commit: `bbc38654bd593d4ae70143230ea7814b34d09128`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 3; wall time 2.4 to 5.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 0.5 | 2.5 | 1 | 1 | [run](https://argusic.com/run/4757118a-5a5c-434f-9610-6da90165a6c1) |
| 2 | fail | 80 | 1 | 5.4 | 5 | 5 | [run](https://argusic.com/run/711be0cc-e4b7-4eb1-af97-d77ff98419f0) |
| 3 | fail | 80 | 0.5 | 2.4 | 2 | 2 | [run](https://argusic.com/run/ad6941f5-6b20-41f6-9daa-7ed9deaa8c6c) |

## What was observed on a clean machine

Attempt 1:

- 0.2 min: `chrome-sandbox SUID sandbox helper not configured correctly (needs root:4755)`

Attempt 2:

- 0.5 min: `electron SUID sandbox helper not configured correctly (not owned by root, mode not 4755)`
- `D-Bus system bus not available in container (no /run/dbus/system_bus_socket)`
- `BlueZ/Floss manager not available in container`
- `dri3 GPU extension not supported on Xvfb`
- `PulseAudio not available, falling back to ALSA`

Attempt 3:

- 0.3 min: `SUID sandbox helper not configured correctly, process aborted`
- 0.3 min: `GPU process crashed repeatedly due to missing GPU in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
