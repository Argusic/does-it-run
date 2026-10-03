# Cataclysm-DDA

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/CleverRaven/Cataclysm-DDA, licensed NOASSERTION, written in C++.

Evidence and recordings: https://argusic.com/subject/cataclysm-dda

## Pinned environment

- Project commit: `98e4c61d936a84bb94babdb00785e14cebfdcba8`
- Test commit: `98e4c61d936a84bb94babdb00785e14cebfdcba8`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 3; wall time 27.1 to 126.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | n/a | 117 | 0 | 0 | [run](https://argusic.com/run/f44463f6-03e6-40a7-8413-1e93c7860791) |
| 1 | pass | 100 | 27 | 27.1 | 1 | 1 | [run](https://argusic.com/run/1a3b21ba-13c9-4540-b8ac-40b039ae7b3a) |
| 2 | timeout | none | 120 | 126.6 | 4 | 4 | [run](https://argusic.com/run/c6f8acb9-3e27-488e-9a94-20c8ff674f87) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `libncursesw5-dev development headers not installed in container (no root access for apt)`

Attempt 2:

- 10 min: `Missing ncurses headers (ncurses.h, curses.h)`
- 2 min: `Missing zlib headers (zconf.h, zlib.h)`
- 1 min: `Missing zlib .so for linking (-lz not found)`
- 1 min: `Missing bzip2 headers (bzlib.h)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
