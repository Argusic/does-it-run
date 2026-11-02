# tmux

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/tmux/tmux, licensed ISC, written in C.

Evidence and recordings: https://argusic.com/subject/tmux

## Pinned environment

- Project commit: `a7a3b4b3a8066a826a0d57a47c66bdf1d9475cac`
- Test commit: `a7a3b4b3a8066a826a0d57a47c66bdf1d9475cac`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 7.9 to 17.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8 | 7.9 | 4 | 4 | [run](https://argusic.com/run/2e308825-a95c-4af6-89b2-d9600076e94f) |
| 2 | pass | 100 | 18 | 17.9 | 5 | 5 | [run](https://argusic.com/run/83992f8a-e95f-4282-8f6d-f2032bce07c1) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Missing autotools (autoconf, automake, bison, m4)`
- 3 min: `Perl scripts had hardcoded /usr paths`
- 1 min: `Configure failed with PKG_CHECK_MODULES unexpanded`
- 1 min: `make failed: bison data files not found`

Attempt 2:

- 5 min: `Missing build tools (autoconf, automake, bison, m4) and libraries (libevent-dev, libncurses-dev)`
- 3 min: `aclocal-1.16 hardcoded /usr/share/aclocal-1.16 and couldn't find Automake perl modules`
- 2 min: `autom4te failed: autom4te.cfg had hardcoded /usr/share/autoconf paths`
- 1 min: `autoconf and autoheader had hardcoded /usr/share/autoconf paths for trailer.m4`
- 2 min: `bison couldn't find m4 (/usr/bin/m4 hardcoded) or share/bison directory`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
