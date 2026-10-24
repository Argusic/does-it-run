# audiotext

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/HenestrosaDev/audiotext, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/audiotext

## Pinned environment

- Project commit: `b0c5e5092871413c7a8f242da5ad3f4bd767ce8b`
- Test commit: `b0c5e5092871413c7a8f242da5ad3f4bd767ce8b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 8.4 to 8.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 9 | 8.4 | 2 | 2 | [run](https://argusic.com/run/efa56f02-99d1-4746-9382-a3638534774f) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Missing system packages: python3-tk, libtk8.6, libtcl8.6, tk8.6-blt2.5 (tkinter not available for Python 3.12)`
- 1 min: `Missing system package: libportaudio2 (sounddevice could not find PortAudio)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
