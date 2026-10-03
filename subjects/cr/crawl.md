# crawl

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/crawl/crawl, licensed NOASSERTION, written in C++.

Evidence and recordings: https://argusic.com/subject/crawl

## Pinned environment

- Project commit: `749c9a513a2d1ee040e4e534f7b522fb02834b77`
- Test commit: `749c9a513a2d1ee040e4e534f7b522fb02834b77`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 3; wall time 26.1 to 42 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | n/a | 42 | 0 | 0 | [run](https://argusic.com/run/e0831be7-8e7b-4a72-9dd6-068fbb0bf254) |
| 1 | pass | 100 | 40 | 26.1 | 5 | 5 | [run](https://argusic.com/run/2061d46c-f66f-4147-910d-848e8d9eae2e) |
| 2 | timeout | none | n/a | 42 | 0 | 0 | [run](https://argusic.com/run/e754b727-ad26-4360-8f5e-4838c905637c) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Missing PyYAML Python module required by build code generators`
- 15 min: `Missing libncursesw-dev headers (no root to apt install)`
- 1 min: `Missing zlib.h, lua.h, sqlite3.h, pcre.h system development headers`
- 1 min: `git describe failed (no tags in shallow clone) preventing version header generation`
- 1 min: `ncurses headers installed to include/ but Makefile expected include/ncursesw/ subdirectory`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
