# rats-search

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/librats/rats-search, licensed MIT, written in C++.

Evidence and recordings: https://argusic.com/subject/rats-search

## Pinned environment

- Project commit: `29b5c64f8e4e9e17017d6188845c90bac1d4182b`
- Test commit: `29b5c64f8e4e9e17017d6188845c90bac1d4182b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 9.4 to 13.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 9.4 | 1 | 1 | [run](https://argusic.com/run/dab1ad00-2209-4000-b65a-cb6b2bfdf958) |
| 2 | pass | 100 | 13 | 13.8 | 5 | 5 | [run](https://argusic.com/run/af6aaa96-c4b9-4e81-9a90-388be08c5705) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Qt6 development packages (qt6-base-dev, qt6-websockets-dev, qt6-base-dev-tools, qmake6, qt6-l10n-tools, qt6-tools-dev, linguist-qt6, libxkbcommon-dev, libproxy1v5/libproxy-dev, libduktape207, libqt6sql6-mysql, libqt6test6t64) not installed`

Attempt 2:

- 4 min: `Qt6 development packages not installed (only runtime libs available from system packages, version 6.4.2 lacks WebSockets dev headers)`
- 3 min: `Missing OpenGL development headers and libraries (Qt6Gui requires GL/gl.h, libGL.so, libX11 headers)`
- 3 min: `CMake FindOpenGL with GLVND creates OpenGL::OpenGL but Qt 6.9.2's FindWrapOpenGL expects OpenGL::GL`
- 1 min: `QMYSQL SQL driver cannot load: libmysqlclient.so.21 not found`
- 1 min: `Tests crash on xcb platform plugin (no display)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
