# engine

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/g3n/engine, licensed BSD-2-Clause, written in Go.

Evidence and recordings: https://argusic.com/subject/engine

## Pinned environment

- Project commit: `83026d7a122877e722885090410c002ffae6defc`
- Test commit: `83026d7a122877e722885090410c002ffae6defc`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 31.1 to 31.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 29 | 31.1 | 5 | 5 | [run](https://argusic.com/run/d892ecbd-e3f3-4a74-831e-67d9d87a3d87) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Go compiler not installed in container`
- 8 min: `Missing C -dev headers (X11, GL, OpenAL, Vorbis, etc.) at /usr/include`
- 2 min: `CGo include paths in audio packages pointed to /usr/include which lacks headers`
- 4 min: `Linker could not find -lGL, -lX11, etc. (no -dev .so symlinks)`
- 1 min: `Stray sources.go at repo root shadowed renderer/shaders/sources.go and caused 'undefined: ProgramInfo'`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
