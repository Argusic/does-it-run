# olive

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/olive-editor/olive, licensed GPL-3.0, written in C++.

Evidence and recordings: https://argusic.com/subject/olive

## Pinned environment

- Project commit: `7e0e94abf6610026aebb9ddce8564c39522fac6e`
- Test commit: `7e0e94abf6610026aebb9ddce8564c39522fac6e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, no run possible
- Valid runs: 3; wall time 30.3 to 73.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 73 | 73.6 | 5 | 5 | [run](https://argusic.com/run/528b9707-6eed-4c6c-868d-3072da5412c3) |
| 2 | timeout | none | n/a | 42 | 0 | 0 | [run](https://argusic.com/run/d70449e6-2d26-4955-af8b-3191251a78c8) |
| 3 | pass | 100 | 23 | 30.3 | 6 | 6 | [run](https://argusic.com/run/6932d217-bd8c-4e70-a8f5-764f23cdf906) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Missing Qt6 development headers and cmake configs - only runtime libs were installed`
- 15 min: `Missing OpenGL, FFmpeg, OpenColorIO, OpenImageIO, OpenEXR, Imath, PortAudio, Zlib, XKB development headers/libraries`
- 5 min: `Cmake config files from Debian packages had incorrect absolute paths referencing /usr/lib/x86_64-linux-gnu instead of our sysroot`
- 2 min: `QStringRef was removed in Qt6 causing compilation error in serializer230220.cpp`
- 30 min: `OpenImageIO and OpenCV had dozens of transitive shared library dependencies (GDAL, OpenVDB, DCMTK, OpenCV, etc.) that required hundreds of MB of additional runtime libs`

Attempt 3:

- 2 min: `OpenGL headers/libs not found (no -dev packages in container)`
- 4 min: `Qt6 cmake modules missing; qmake wrapper script used absolute /usr/lib/qt6/bin/qmake which didn't exist`
- 1 min: `Git submodules (ext/core, ext/KDDockWidgets) not cloned`
- 1 min: `QStringRef removed in Qt6 (serializer230220.cpp)`
- 2 min: `FindFFMPEG.cmake chose .a static libs over .so, causing soxr/other link errors`
- 13 min: `OIIO/OCIO transitive shared libs missing (opencv, dcmtk, boost, gstreamer, gphoto2, gdal, blosc, openvdb, etc., ~100 debs)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
