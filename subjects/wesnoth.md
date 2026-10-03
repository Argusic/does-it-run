# wesnoth

**Verdict: runs.** Argusic Score 66.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/wesnoth/wesnoth, licensed GPL-2.0, written in C++.

Evidence and recordings: https://argusic.com/subject/wesnoth

## Pinned environment

- Project commit: `9de04e8dd928e433bf0c571a58547dfb6a75b46c`
- Test commit: `9de04e8dd928e433bf0c571a58547dfb6a75b46c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 4; wall time 20 to 68.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | n/a | 42 | 0 | 0 | [run](https://argusic.com/run/4230b926-9a1e-4272-9da2-d63888b44e6d) |
| 1 | fail | 80 | 37 | 41 | 6 | 6 | [run](https://argusic.com/run/0e5bd651-da0a-4aad-9b8a-da06183fbe13) |
| 2 | fail | 20 | 5 | 20 | 1 | 1 | [run](https://argusic.com/run/d9a34d8b-4dbe-4049-a5aa-39d6eb0e1650) |
| 2 | pass | 100 | 64 | 68.4 | 4 | 4 | [run](https://argusic.com/run/f64222a9-5b05-49aa-85b8-1b90146b934a) |

## What was observed on a clean machine

Attempt 1:

- 16 min: `Missing boost libraries (1.83.0 required)`
- 1 min: `Lua submodule not initialized`
- 4 min: `Missing ICU dev headers/lib symlinks for cmake`
- 5 min: `Boost iostreams built without zlib/bzip2 support`
- 1 min: `Boost include paths not propagated to wesnoth-common target`
- 4 min: `SDL3, CURL, Fontconfig, Pango/Cairo dev libraries unavailable (no root) - needed for game and test targets`

Attempt 2:

- 5 min: `Source build requires SDL3 (not available in Ubuntu 24.04 repos), Boost dev headers, Pango/Cairo/Fontconfig dev headers. No root access to install system packages. Cannot install apt -dev packages.`

Attempt 2:

- 15 min: `Boost headers not picked up by cmake include_directories; cmake found Boost via config mode but include paths were not propagated to compiler flags`
- 25 min: `pkg-config transitive dependencies missing for pangocairo, fontconfig, cairo (missing proto .pc files, libffi, libpcre2, etc.)`
- 20 min: `SDL3 required by project but not available in apt for Ubuntu 24.04`
- 5 min: `SDL video initialization failed during test execution - no video device available`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
