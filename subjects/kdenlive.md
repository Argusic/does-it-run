# kdenlive

**Verdict: runs with mocks.** Argusic Score 33.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/KDE/kdenlive, licensed GPL-3.0, written in C++.

Evidence and recordings: https://argusic.com/subject/kdenlive

## Pinned environment

- Project commit: `b7124d97e8f810d9170b7049837cd7ac84edd522`
- Test commit: `b7124d97e8f810d9170b7049837cd7ac84edd522`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run, run with mocked services
- Valid runs: 3; wall time 12.8 to 90.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 8 | 98 | 90.9 | 5 | 2 | [run](https://argusic.com/run/880bf604-dcc1-40e1-a6e9-3b407281d5f2) |
| 2 | fail | 0 | 0 | 12.8 | 1 | 0 | [run](https://argusic.com/run/cd0b5dd6-5577-414b-bb38-ee95f8921e02) |
| 2 | pass with mocks | 92 | 85 | 46.1 | 5 | 5 | [run](https://argusic.com/run/fec0dff0-e2c1-4cc4-86e7-2262e219de5a) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Required Qt 6.10+ but only Qt 6.8.0 available via aqtinstall`
- 60 min: `Required KF6 6.21+ but only KF6 6.8.0 available in stable tags; failed to build 9 of 20 required frameworks`
- 15 min: `KF6 Solid build required FLEX (fixed) but also UDev headers (unavailable); KF6 Notifications required libcanberra; KF6 TextWidgets required KF6Sonnet (which needed hunspell and failed to link)`
- 12 min: `MLT 7.22.0 from apt but required 7.38+; built MLT 7.38 from source with reduced features (no SDL2, no OpenCV, no QT6)`
- 5 min: `System has 50GB memory and 4 cores but no root access; cannot install -dev packages via apt`

Attempt 2:

- `Kdenlive requires Qt >= 6.10, KF6 >= 6.21, MLT >= 7.38, KDDockWidgets >= 2.4.0 and many more KDE libraries that are not available as development packages in the container (Ubuntu 24.04 LTS with Qt 6.4.2). Cannot install system packages (no`

Attempt 2:

- 30 min: `CMake found Qt 6.4.2 on system but Kdenlive requires Qt 6.10+ and KF6 6.21+. Installed Qt 6.12 via aqtinstall, built ECM 6.31 from source, extracted MLT 7.22/FFmpeg dev packages from distro .debs.`
- 30 min: `KF6 frameworks (18+ modules) are not available as packages on Ubuntu 24.04 and cannot be built from source in the time budget`
- 10 min: `C++ compilation of kdenliveLib fails due to hundreds of missing KF6 header files (KPluginFactory, KLocalizedString, KMessageWidget, KActionCategory, etc.) that cannot be fully stubbed`
- 5 min: `CMake qml lint step fails due to missing org.kde.ki18n QML module`
- 5 min: `kdenlive_render binary requires QT_QPA_PLATFORM=offscreen to run due to missing xcb-cursor0 runtime library`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
