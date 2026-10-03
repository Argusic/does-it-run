# valkey

**Verdict: runs.** Argusic Score 96.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/valkey-io/valkey, licensed BSD-3-Clause, written in C.

Evidence and recordings: https://argusic.com/subject/valkey

## Pinned environment

- Project commit: `85d02f6388805948a638c8f3375db63a9800b8d9`
- Test commit: `85d02f6388805948a638c8f3375db63a9800b8d9`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 3; wall time 15.5 to 51.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 9 | 15.5 | 4 | 4 | [run](https://argusic.com/run/a666864f-63d7-42d2-96b9-c1f14ff2e664) |
| 2 | pass | 90 | 18 | 15.5 | 2 | 1 | [run](https://argusic.com/run/78c8e755-080a-4508-bace-e31daeac2059) |
| 3 | pass | 100 | 42 | 51.3 | 3 | 3 | [run](https://argusic.com/run/5a94bdfd-0223-408c-bec4-66ee33e09c5a) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Makefile typo: 'QUITE_GEN' should be 'QUIET_GEN' on lines 784-786 of src/Makefile causes fmtargs.h generation to fail`
- 5 min: `googletest not installed (no root). Unit tests cannot build or run without it`
- 1 min: `Tcl not installed (no root). Integration tests require Tcl (tclsh) and cannot run`
- `Unit test suite has pre-existing test pollution causing 17 failed tests and 1 segfault when run together (all pass in isolation)`

Attempt 2:

- 1 min: `Unit tests required googletest, which was not installed`
- `Integration tests require tclsh 8.5+, which was not installed and cannot be installed (no root)`

Attempt 3:

- 5 min: `googletest not found for unit tests`
- 3 min: `tcl not installed (no root)`
- 2 min: `unit test -Werror=float-equal breaks gmock headers`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
