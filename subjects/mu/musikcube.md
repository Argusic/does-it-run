# musikcube

**Verdict: runs.** Argusic Score 66.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/clangen/musikcube, licensed BSD-3-Clause, written in C++.

Evidence and recordings: https://argusic.com/subject/musikcube

## Pinned environment

- Project commit: `9bc1234c8c36e40e255bc3878c0eba2c82b9cdeb`
- Test commit: `9bc1234c8c36e40e255bc3878c0eba2c82b9cdeb`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 3; wall time 24.2 to 70.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 70.8 | 0 | 0 | [run](https://argusic.com/run/98048138-5681-48d7-88a9-6e691b08b579) |
| 2 | pass | 100 | 25 | 26.3 | 5 | 5 | [run](https://argusic.com/run/0c7273fb-dd4c-4c1c-98e1-b517af1d3952) |
| 3 | fail | 80 | 24 | 24.2 | 5 | 5 | [run](https://argusic.com/run/87b282d8-29e5-4b0c-9cff-5c8c25000239) |

## What was observed on a clean machine

Attempt 2:

- 0.2 min: `Missing git submodules (asio, musikcube-bin)`
- 3 min: `No -dev packages installed (root not available)`
- 5 min: `Static libraries (.a) not compiled with -fPIC, caused linker errors when building .so plugins and libmusikcore.so`
- 2 min: `Header files in multiarch directory (x86_64-linux-gnu) not found by compiler`
- 3 min: `Cmake find_library couldn't find libtag, libcurl, libncursesw, libev, libmicrohttpd, ffmpeg libs`

Attempt 3:

- 2 min: `Git submodules src/3rdparty/asio and src/3rdparty/bin not initialized`
- 6 min: `No root/sudo - can't apt-get install -dev packages`
- 1 min: `libz.a compiled without -fPIC; cannot link into shared library libmusikcore.so`
- 1 min: `taglib includes not found - source uses #include <taglib/tlist.h>`
- 3 min: `Broken .so symlinks - dev packages only provide .so -> .so.N links but not the .so.N targets`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
