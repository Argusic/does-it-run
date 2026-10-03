# cubrid

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/CUBRID/cubrid, licensed Apache-2.0, written in C.

Evidence and recordings: https://argusic.com/subject/cubrid

## Pinned environment

- Project commit: `e374c7a24c46449c3f79e9413a6f4ff3d23b16c2`
- Test commit: `e374c7a24c46449c3f79e9413a6f4ff3d23b16c2`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, no run possible
- Valid runs: 2; wall time 8.7 to 73.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 72 | 73.3 | 11 | 11 | [run](https://argusic.com/run/ec60745d-5320-4ac0-9dc9-e37ffb3e7f4b) |
| 2 | fail | 20 | n/a | 8.7 | 0 | 0 | [run](https://argusic.com/run/a65fbbb4-c5b4-4e7b-ac0f-b631cdd61070) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `Missing flex and bison tools`
- 2 min: `Missing JDK (Java required for PL engine)`
- 1 min: `CMake: dtrace/systemtap not found`
- 3 min: `CMake: Ant not found for JDBC build`
- 3 min: `CMake: JNI not found (JAVA_HOME pointing to non-existent JDK8)`
- 10 min: `3rdparty libedit: requires libncurses (only libncursesw available)`
- 5 min: `3rdparty libtbb: GCC 13 -Werror=stringop-overflow`
- 3 min: `3rdparty libodbc: VERSION macro undefined`
- 1 min: `porting.c: missing curses.h header`
- 2 min: `dynamic_load.c: missing nlist.h header`
- 5 min: `dblink_scan.c: missing CCI headers and library (CCI disabled)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
