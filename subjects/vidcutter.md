# vidcutter

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ozmartian/vidcutter, licensed GPL-3.0, written in Python.

Evidence and recordings: https://argusic.com/subject/vidcutter

## Pinned environment

- Project commit: `db6818f11bbb4d5598dfc5ceeddf7f81c7078499`
- Test commit: `db6818f11bbb4d5598dfc5ceeddf7f81c7078499`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 11.8 to 14.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 2 | pass | 100 | 20 | 14.8 | 6 | 6 | [run](https://argusic.com/run/da24434b-2424-4a46-9def-1fe7d2f7354d) |
| 2 | pass | 100 | 12 | 11.8 | 12 | 12 | [run](https://argusic.com/run/a62ca65e-8b0e-46ab-b21d-042c0e15448b) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `System missing python3-dev headers (Python.h)`
- 2 min: `System missing libmpv2 and libmpv-dev`
- 3 min: `libmpv runtime deps missing (dvdnav, mujs, lua5.2, sixel, xpresent, va-wayland, dvdread, xcb-xinerama)`
- 2 min: `Externally managed Python - pip install blocked`
- 1 min: `C build missing pyconfig.h multiarch include path`
- 1 min: `xcb platform plugin failed due to missing libxcb-xinerama`

Attempt 2:

- 1 min: `pip install failed: externally-managed-environment`
- 0.5 min: `setup.py build_ext: ModuleNotFoundError: No module named 'setuptools'`
- 2 min: `setup.py build_ext: fatal error: Python.h: No such file or directory`
- 1 min: `setup.py build_ext: fatal error: x86_64-linux-gnu/python3.12/pyconfig.h`
- 0.5 min: `setup.py build_ext: fatal error: mpv/client.h: No such file or directory`
- 1 min: `runtime: ImportError: libdvdnav.so.4: cannot open shared object file`
- 0.5 min: `runtime: ImportError: libmujs.so.3 not found`
- 0.5 min: `runtime: ImportError: liblua5.2.so.0 not found`
- 0.5 min: `runtime: ImportError: libsixel.so.1 not found`
- 0.5 min: `runtime: ImportError: libXpresent.so.1 not found`
- 0.5 min: `runtime: ImportError: libva-wayland.so.2 not found`
- 0.5 min: `runtime: ImportError: libdvdread.so.8 not found (transitive dep of libdvdnav)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
