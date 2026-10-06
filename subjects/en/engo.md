# engo

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/EngoEngine/engo, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/engo

## Pinned environment

- Project commit: `4d9de92353879edf4d7597d6070f4994cf307c41`
- Test commit: `4d9de92353879edf4d7597d6070f4994cf307c41`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 17.1 to 17.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 16 | 17.1 | 9 | 9 | [run](https://argusic.com/run/7dcfd298-f8fc-42f6-bb61-b5bcf6ed7bf5) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go not found in container`
- 3 min: `X11/Xlib.h missing for glfw C compilation`
- 1 min: `X11/X.h not found (included by Xlib.h)`
- 1 min: `X11/extensions/Xrender.h missing`
- 2 min: `X11/extensions/Xfixes.h missing`
- 1 min: `pkg-config gl.pc not found`
- 1 min: `GL/glx.h header missing`
- 2 min: `Linker cannot find -lGL, -lasound, -lXxf86vm`
- 1 min: `libX11.a static library has unresolved xcb symbols`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
