# flowblade

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/jliljebl/flowblade, licensed GPL-3.0, written in Python.

Evidence and recordings: https://argusic.com/subject/flowblade

## Pinned environment

- Project commit: `1ffef10a791690501ae09cb3c4e0fce8fb0951dd`
- Test commit: `1ffef10a791690501ae09cb3c4e0fce8fb0951dd`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 12.9 to 30.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 23.1 | 30.3 | 6 | 6 | [run](https://argusic.com/run/0fb479fd-2511-4c8d-ae4b-5261de672a96) |
| 2 | pass with mocks | 92 | 8 | 12.9 | 6 | 6 | [run](https://argusic.com/run/4b9af9a7-fe2b-4d85-90ce-01faadc6db7f) |

## What was observed on a clean machine

Attempt 1:

- 10 min: `Missing Python dependencies (pygobject, pycairo, mlt, numpy, Pillow, usb1) - not installed in container`
- 2 min: `MLT plugins not found - system MLT library looked in wrong path`
- 3 min: `Introspection typelib chain errors (xlib, Atk, HarfBuzz namespaces not found)`
- 2 min: `editorlayout.py bug: _panel_positions is None on fresh install`
- 1 min: `editorwindow.py bug: G'MIC widget access on None`
- 3 min: `Missing optional MLT plugin dependencies (libexif, Qt5, movit, opencv, frei0r, LADSPA)`

Attempt 2:

- 2 min: `No root access to install system packages via apt`
- 2 min: `Python dependencies missing: gi, mlt, PIL, numpy, cairo, usb1`
- 1 min: `Missing shared libraries: libgirepository, libmlt, libimagequant, frei0r plugins`
- 1 min: `Missing GObject introspection typelibs for Gtk, Pango, Atk, HarfBuzz, Xlib`
- 1 min: `editorlayout.py: panel_positions is None on first launch, try/except attempts to index into None`
- 0.5 min: `editorwindow.py: Gtk.UIManager.get_widget() returns None for G'Mic menu item when gmic unavailable`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
