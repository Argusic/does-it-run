# kohi

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/travisvroman/kohi, licensed Apache-2.0, written in C.

Evidence and recordings: https://argusic.com/subject/kohi

## Pinned environment

- Project commit: `34e51506f8083b382ed857a4ccb69f75e89fea6b`
- Test commit: `34e51506f8083b382ed857a4ccb69f75e89fea6b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 44.5 to 44.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 42 | 44.5 | 5 | 5 | [run](https://argusic.com/run/21fd258f-e15a-4692-8c69-34001c590e48) |

## What was observed on a clean machine

Attempt 1:

- 10 min: `No clang compiler in container (GCC only)`
- 5 min: `Source code uses __gcc__ compiler detection macro which GCC does not define (uses __GNUC__ instead)`
- 15 min: `Missing X11, xcb, xkbcommon, systemd development headers for platform_linux.c`
- 7 min: `GCC treats warnings as errors that clang does not (fallthrough, type-limits, sign-compare, return-type, etc.)`
- 5 min: `Platform_linux.c references CLOCK_MONOTONIC_RAW and xcb_xkb functions unavailable with header stubs`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
