# nnn

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/jarun/nnn, licensed BSD-2-Clause, written in C.

Evidence and recordings: https://argusic.com/subject/nnn

## Pinned environment

- Project commit: `fcd794631106197e94e131ef5b04a1bbdfd447a1`
- Test commit: `fcd794631106197e94e131ef5b04a1bbdfd447a1`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 3; wall time 8.2 to 29.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 29 | 29.7 | 3 | 3 | [run](https://argusic.com/run/7da49073-fd96-4682-8d6f-857e86c7d74f) |
| 2 | pass | 100 | 18 | 18 | 2 | 2 | [run](https://argusic.com/run/346d71bd-d515-4228-a057-acadf1e662fe) |
| 3 | pass | 100 | 6 | 8.2 | 3 | 3 | [run](https://argusic.com/run/48beda59-b6db-4523-9885-ac227af327dd) |

## What was observed on a clean machine

Attempt 1:

- 22 min: `No C compiler (gcc/cc) installed in container`
- 2 min: `Missing ncurses development headers (libncurses-dev)`
- 2 min: `Missing linux kernel headers (sys/inotify.h)`

Attempt 2:

- 2 min: `Missing libncurses-dev (curses.h header and linker scripts)`
- 5 min: `Dynamic link binary crashed with 'corrupted size vs. prev_size' heap corruption`

Attempt 3:

- 2 min: `curses.h: No such file or directory during compilation`
- 1 min: `cannot find -lncurses at link time`
- 3 min: `Binary crashed with corrupted size vs. prev_size (SIGABRT)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
