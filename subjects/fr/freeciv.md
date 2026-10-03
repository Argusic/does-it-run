# freeciv

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/freeciv/freeciv, licensed GPL-2.0, written in C.

Evidence and recordings: https://argusic.com/subject/freeciv

## Pinned environment

- Project commit: `af1c40980e633969e5bc0ed2338cd267cf0ad409`
- Test commit: `af1c40980e633969e5bc0ed2338cd267cf0ad409`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 12.7 to 18.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 18.3 | 4 | 4 | [run](https://argusic.com/run/5eaec724-b39b-4c5a-9239-0eac3fb13772) |
| 2 | pass | 100 | 12 | 12.7 | 5 | 5 | [run](https://argusic.com/run/f39c5904-c92d-40c6-acb6-db5ce1379a1a) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `meson/ninja not installed (missing build system)`
- 6 min: `Missing -dev packages: zlib1g-dev, libpng-dev, libsqlite3-dev, libicu-dev, libcurl4-openssl-dev`
- 3 min: `ICU static libs not compiled with -fPIC, cannot link into shared libfreeciv.so`
- 1 min: `Server can't find ruleset data files when run directly`

Attempt 2:

- 1 min: `meson and ninja not installed`
- 1 min: `zlib development headers not found`
- 1 min: `icu-uc development package not found`
- 1 min: `curl development library not found`
- 1 min: `sqlite3 development library not found`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
