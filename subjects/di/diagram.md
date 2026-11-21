# diagram

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/esimov/diagram, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/diagram

## Pinned environment

- Project commit: `ffabf939b33492e4c6e5a1565a658f4ff751e480`
- Test commit: `ffabf939b33492e4c6e5a1565a658f4ff751e480`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 3.7 to 14 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 14 | 14 | 4 | 4 | [run](https://argusic.com/run/1c6ff341-195a-464d-ba9d-bb1d9370df0a) |
| 2 | pass | 100 | 1.58 | 3.7 | 2 | 2 | [run](https://argusic.com/run/29d7934b-2a4e-48c1-8b70-c57191f20ad9) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `go toolchain not installed in container`
- 25 min: `missing X11/xkbcommon/wayland/EGL/Vulkan dev headers and .pc files needed by Gio cgo build`
- 5 min: `link failed: cannot find -lEGL/-lwayland-client/-lxkbcommon and undefined XRender/Xext/Xau symbols`
- 10 min: `preview window log spammed 1700+ MESA: error: Failed to attach to x11 shm lines under Xvfb`

Attempt 2:

- 0.1 min: `Go (golang) is not installed in the container`
- 1 min: `CGo dependencies missing: xkbcommon, wayland-client, EGL, Vulkan and X11 dev headers not found (no root to install libxkbcommon-dev etc.)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
