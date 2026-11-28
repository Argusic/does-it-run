# ned

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/nealmick/ned, licensed MIT, written in C++.

Evidence and recordings: https://argusic.com/subject/ned

## Pinned environment

- Project commit: `2d3e9b53b0ebc44c6da6901ff242a95edaa4a1ff`
- Test commit: `2d3e9b53b0ebc44c6da6901ff242a95edaa4a1ff`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 26.1 to 26.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 25 | 26.1 | 8 | 8 | [run](https://argusic.com/run/5ee204cc-e14e-49f2-8187-88e13d0b6ef0) |

## What was observed on a clean machine

Attempt 1:

- 6 min: `Missing development packages (glfw3, glew, freetype, fontconfig, curl, gtk+3, glib, cairo, pango, etc)`
- 4 min: `Missing CMake find modules for glfw3 and GLEW, and broken FindCURL doesn't set IMPORTED_LOCATION`
- 3 min: `Tree-sitter submodules not initialized (empty directories)`
- 6 min: `GTK3 pkg-config dependency chain incomplete (missing .pc for dozens of transitive deps like xproto, mount, libjpeg, etc)`
- 3 min: `Missing runtime .so versioned files (/tmp/local had dev .so symlinks to .so.N that didn't exist)`
- 1 min: `OpenGL not found correctly (OPENGL_gl_LIBRARY not set, libGL.so missing symlink in system)`
- 1 min: `Missing glibconfig.h in glib-2.0 include dir`
- 1 min: `libGLU.a not found at expected /tmp/local/lib/x86_64-linux-gnu/ path`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
