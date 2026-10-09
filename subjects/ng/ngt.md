# NGT

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/NGT-labs/NGT, licensed Apache-2.0, written in C++.

Evidence and recordings: https://argusic.com/subject/ngt

## Pinned environment

- Project commit: `573dab62b78352251f42f74ece94bb27ab641a5b`
- Test commit: `573dab62b78352251f42f74ece94bb27ab641a5b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 10.7 to 10.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 4 | 10.7 | 3 | 3 | [run](https://argusic.com/run/556da260-9421-43ce-ac67-73a5291d7e28) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `make install: Permission denied writing to /usr/local/lib`
- 2 min: `Python ngtpy C++ extension build failed: python3-dev (Python.h) not available on system and cannot be installed without root`
- 1 min: `Python ngtpy C++ extension build failed: missing generated headers defines.h and version_defs.h in include path`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
