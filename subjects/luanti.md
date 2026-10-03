# luanti

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/luanti-org/luanti, licensed NOASSERTION, written in C++.

Evidence and recordings: https://argusic.com/subject/luanti

## Pinned environment

- Project commit: `b81bb3c68ac633f1df8dd8ed758644cabf4c1efd`
- Test commit: `b81bb3c68ac633f1df8dd8ed758644cabf4c1efd`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 3; wall time 11.1 to 56.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 21.5 | 22 | 3 | 3 | [run](https://argusic.com/run/0577847d-bb8a-4367-b098-587403692b33) |
| 2 | pass | 100 | 55 | 56.9 | 6 | 6 | [run](https://argusic.com/run/c4071d5d-03d5-40fe-a701-67eefb7019ce) |
| 3 | pass | 100 | 12 | 11.1 | 3 | 3 | [run](https://argusic.com/run/e2937c07-9dd1-42e9-a754-02c5aa8a2d90) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `Missing system -dev packages (libsqlite3-dev, zlib1g-dev, libzstd-dev, etc.) - no root access to install them`
- 5 min: `No network connectivity in container (archive.ubuntu.com unreachable)`
- 1 min: `2 unit test failures: testIPv6Socket and testResolve (DNS)`

Attempt 2:

- 10 min: `Missing dev headers - no root to apt-get install`
- 3 min: `SDL2 include path missing arch-specific x86_64-linux-gnu dir`
- 1 min: `libGL symlink broken in devroot (pointed to missing libGL.so.1)`
- 2 min: `Static libcurl pulled kerberos/GSSAPI link deps`
- 1 min: `Static libfreetype pulled brotli link deps`
- 2 min: `Linker couldn't find -lasound and other SDL2 private libs`

Attempt 3:

- 8 min: `Missing -dev packages for sqlite3, zstd, zlib, png, jpeg, sdl2, freetype, luajit, ogg, vorbis, openal, curl, gmp, jsoncpp, ncurses, mesa, gettext`
- 2 min: `find_symbol_exists(ZSTD_initCStream) failed during CMake configure because check_symbol_exists could not link against the static lib`
- 1 min: `Missing libz.so.1.3 and libzstd.so.1.5.5 shared libraries in local sysroot (symlinks pointed to non-existent files)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
