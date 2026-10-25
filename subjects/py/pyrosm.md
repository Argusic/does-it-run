# pyrosm

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/pyrosm/pyrosm, licensed BSD-3-Clause, written in Python.

Evidence and recordings: https://argusic.com/subject/pyrosm

## Pinned environment

- Project commit: `ea1eff44e0848a9c8a7189ff979f6215b81e5fa6`
- Test commit: `ea1eff44e0848a9c8a7189ff979f6215b81e5fa6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 29.2 to 29.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 36 | 29.2 | 5 | 5 | [run](https://argusic.com/run/5b6d5cd9-9881-45c2-a494-be1e9fed34b8) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `Python.h missing , system python3-minimal does not ship CPython headers; gcc cannot compile Cython extensions`
- 3 min: `cykhash build failed without Python.h include path`
- 2 min: `pyrosm source build failed with Cython.Compiler.Errors.CompileError on data_filter.pyx (cykhash not importable)`
- 1 min: `Tests failed because repo pyrosm/ dir (without .so) shadowed installed C extensions`
- 1 min: `Optional dependencies missing , pyarrow, python-igraph, networkx`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
