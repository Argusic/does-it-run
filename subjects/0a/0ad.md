# 0ad

**Verdict: could not verify.** Argusic Score 18.6 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/0ad/0ad, licensed NOASSERTION, written in C++.

Evidence and recordings: https://argusic.com/subject/0ad

## Pinned environment

- Project commit: `61a3b9507d974084e6badb88a0826bd89a6d5b8b`
- Test commit: `61a3b9507d974084e6badb88a0826bd89a6d5b8b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 4; wall time 33.4 to 61.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | n/a | 42 | 0 | 0 | [run](https://argusic.com/run/15caacf8-16e5-4ff0-b7e9-82810a556e55) |
| 1 | fail | 20 | 51 | 61.3 | 2 | 2 | [run](https://argusic.com/run/7c49b658-925d-4dc5-9752-5ad0a54e9d0b) |
| 2 | timeout | none | 40 | 43 | 3 | 3 | [run](https://argusic.com/run/a3f8b8d5-9983-4188-9476-ad481c6956eb) |
| 2 | fail | 17.14 | 120 | 33.4 | 7 | 6 | [run](https://argusic.com/run/19c34cdc-acd7-4d8f-ba3a-b6f02169729a) |

## What was observed on a clean machine

Attempt 1:

- 40 min: `SpiderMonkey mozjs-91 build failed: the Mozilla build system requires many Python dependencies not available (mozversioncontrol, mozprocess, mozfile, etc.) and creating a working Python virtualenv failed. The bundled source tarball was extr`
- 10 min: `Missing development headers for SDL2, libcurl, libxml2, freetype2, OpenAL, etc. No root access to install packages via apt.`

Attempt 2:

- 25 min: `SpiderMonkey (mozjs-91.13.1) build fails: bundled virtualenv v20.x uses distutils and entry_points().get() API, both removed in Python 3.12. Patching six.moves, distutils→setuptools._distutils, and sys.path filter resolved import errors but`
- 5 min: `Cannot apt install packages (no root)`
- 8 min: `No rustc available`

Attempt 2:

- 30 min: `Missing development packages (libxml2-dev, libsdl2-dev, libboost-dev, libfmt-dev, libgloox-dev, libopenal-dev, libx11-dev, libenet-dev, libmozjs-91-dev, etc.) could not be installed via apt-get (no root). Resolved by extracting .deb archive`
- 5 min: `FCollada bundled library build failed: libxml/tree.h not found. Fixed by extracting libxml2-dev into sysroot.`
- 5 min: `Premake5 makefiles didn't include win32 library include paths on Linux. Fixed by patching extern_libs5.lua to set libraries_dir on non-macOS/non-Windows.`
- 5 min: `PCH handling: stale precompiled.h.gch files caused compilation errors. Fixed by cleaning obj directories between builds.`
- 5 min: `Patched pkg-config .pc files to point to /tmp/sysroot/usr instead of /usr.`
- 15 min: `Spidermonkey (mozjs-91): bundled library has only Win32 32-bit headers and .lib files. include-unix-release directory missing. source tarball (70MB) requires autoconf 2.13, Rust, and other build tools not available. Ubuntu 24.04 provides mo`
- 30 min: `The game test runner requires nearly all libraries (including mozjs-dependent scriptinterface/engine/graphics). Without functional SpiderMonkey, the full build and test executable cannot be linked.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
