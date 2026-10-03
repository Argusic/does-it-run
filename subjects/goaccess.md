# goaccess

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/allinurl/goaccess, licensed MIT, written in C.

Evidence and recordings: https://argusic.com/subject/goaccess

## Pinned environment

- Project commit: `5e6a1e4e1976380f9819a899593c399c2a655ccf`
- Test commit: `5e6a1e4e1976380f9819a899593c399c2a655ccf`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 3; wall time 13.7 to 43.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | n/a | 43.2 | 0 | 0 | [run](https://argusic.com/run/817b075f-d05e-4abb-81c7-080370b95421) |
| 2 | pass | 100 | 28 | 27.6 | 4 | 4 | [run](https://argusic.com/run/7e37643c-0ce6-4d05-9609-c08382bb4c18) |
| 3 | pass | 100 | 10 | 13.7 | 2 | 2 | [run](https://argusic.com/run/a3e9817d-242b-4e73-b7f1-927514f7f8cc) |

## What was observed on a clean machine

Attempt 2:

- 8 min: `No C compiler or build tools installed in the container`
- 10 min: `Hardcoded /usr/share/autoconf and /usr/bin/ paths in autotools Perl scripts prevented autoreconf from working`
- 6 min: `Missing gettext infrastructure (autopoint archive, msgfmt with missing libxml2)`
- 2 min: `build-essential and gcc metapackages only contain symlinks, not real binaries`

Attempt 3:

- 3 min: `Missing build toolchain (autoconf, automake, autopoint, gettext, m4) , the git checkout lacks the pre-generated configure script`
- 4 min: `Missing ncurses development headers and shared libraries (libncurses-dev, libncurses6, libtinfo6)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
