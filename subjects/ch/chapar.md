# chapar

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/chapar-rest/chapar, licensed BSD-3-Clause, written in Go.

Evidence and recordings: https://argusic.com/subject/chapar

## Pinned environment

- Project commit: `bfbb761a79d83d37e065f8937a94be650ed21b5e`
- Test commit: `bfbb761a79d83d37e065f8937a94be650ed21b5e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 8 to 8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 7 | 8 | 3 | 3 | [run](https://argusic.com/run/1cf05b93-9631-4aaa-9d08-782c52d03d08) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Go not installed in container`
- 4 min: `Missing X11 and GL development headers for GPU build (X11/Xlib.h, GL/glx.h)`
- 1 min: `Linker could not find -lGL, -lX11, etc. (no .so symlinks in prefix)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
