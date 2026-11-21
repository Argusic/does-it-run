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
- Valid runs: 2; wall time 11.5 to 44.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 42 | 44.5 | 5 | 5 | [run](https://argusic.com/run/21fd258f-e15a-4692-8c69-34001c590e48) |
| 2 | pass | 100 | 24.5 | 11.5 | 10 | 10 | [run](https://argusic.com/run/4bead3ca-1a7b-45d9-a233-8ffaafa6fa7c) |

## What was observed on a clean machine

Attempt 1:

- 10 min: `No clang compiler in container (GCC only)`
- 5 min: `Source code uses __gcc__ compiler detection macro which GCC does not define (uses __GNUC__ instead)`
- 15 min: `Missing X11, xcb, xkbcommon, systemd development headers for platform_linux.c`
- 7 min: `GCC treats warnings as errors that clang does not (fallthrough, type-limits, sign-compare, return-type, etc.)`
- 5 min: `Platform_linux.c references CLOCK_MONOTONIC_RAW and xcb_xkb functions unavailable with header stubs`

Attempt 2:

- 2 min: `No clang compiler available (only gcc)`
- 3 min: `Missing X11 and xkbcommon development headers/libraries`
- 5 min: `GCC-specific compilation errors (-Wgnu-folding-constant, -Werror=inline, -Wno-cast-function-type-mismatch, etc)`
- 3 min: `KINLINE macro caused multiple definition linker errors with -fgnu89-inline`
- 1.5 min: `Missing OpenAL development headers and libraries`
- 1 min: `Missing Vulkan development headers`
- 1.5 min: `Missing shaderc development headers and shared library`
- 3.5 min: `Missing assimp development headers and shared library (plus libdraco8, libpugixml1v5, libminizip1t64 deps)`
- 1 min: `Missing version.txt for kohi.tools module (Makefile referenced non-existent file)`
- 1 min: `kohi.tools Makefile missing -lassimp on Linux link line (symbols from plugin dependency)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
