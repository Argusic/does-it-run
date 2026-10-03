# mopidy

**Verdict: runs.** Argusic Score 46.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/mopidy/mopidy, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/mopidy

## Pinned environment

- Project commit: `0b258eb6c7fd8336b9dce3b8abc3c2c98f235d5d`
- Test commit: `0b258eb6c7fd8336b9dce3b8abc3c2c98f235d5d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 3; wall time 21.6 to 42.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 32.6 | 0 | 0 | [run](https://argusic.com/run/225ca8bc-5348-4f6f-852b-14db39d25712) |
| 2 | fail | 20 | n/a | 42.1 | 0 | 0 | [run](https://argusic.com/run/c44bd5d7-4cf8-44e5-92f5-ffbb4b7688b6) |
| 3 | pass | 100 | 34 | 21.6 | 5 | 5 | [run](https://argusic.com/run/06c9f72d-86b5-4c7e-a772-898c52c56585) |

## What was observed on a clean machine

Attempt 3:

- 25 min: `pygobject/pycairo build failed: missing system deps (cairo, glib, gobject-introspection, dev headers)`
- 2 min: `GStreamer 1.26.2 required but Ubuntu 24.04 only has 1.24.2`
- 2 min: `GStreamer plugin scanner fork lost LD_LIBRARY_PATH, failed to load plugins`
- 3 min: `Missing liborc-0.4.so.0 for GStreamer plugin loading`
- 2 min: `Missing libdw.so.1 for GStreamer ELF handling`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
