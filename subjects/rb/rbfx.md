# rbfx

**Verdict: runs with mocks.** Argusic Score 87 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/rbfx/rbfx, licensed MIT, written in C++.

Evidence and recordings: https://argusic.com/subject/rbfx

## Pinned environment

- Project commit: `d3e8a4ea89e0b2102e3fb4d80751c0e027d1e034`
- Test commit: `d3e8a4ea89e0b2102e3fb4d80751c0e027d1e034`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 80.5 to 80.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 87 | 80 | 80.5 | 4 | 3 | [run](https://argusic.com/run/cf86f3c3-9153-480a-8418-65e6605e97e5) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Missing libdbus-1-dev package prevents building nativefiledialog portal implementation (triggered by URHO3D_TOOLS/URHO3D_EDITOR/URHO3D_PROFILING). Disabled these features.`
- 20 min: `Missing X11/xcb development headers (libx11-dev, libxcb1-dev) cause GLEW and Vulkan backend compilation failures.`
- 5 min: `Missing uuid-dev package causes linker error (uuid_generate, uuid_unparse).`
- `Test crash: Server-client scene loader sequence - Context assertion failure (pre-existing issue).`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
