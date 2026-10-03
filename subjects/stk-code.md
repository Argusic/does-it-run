# stk-code

**Verdict: runs.** Argusic Score 90.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/supertuxkart/stk-code, licensed NOASSERTION, written in C++.

Evidence and recordings: https://argusic.com/subject/stk-code

## Pinned environment

- Project commit: `dbf200ccba14025bac7dc8d0318dcf5e55b6da18`
- Test commit: `dbf200ccba14025bac7dc8d0318dcf5e55b6da18`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run, no run possible
- Valid runs: 3; wall time 19.6 to 28.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 2 | pass with mocks | 92 | 26 | 28.6 | 6 | 6 | [run](https://argusic.com/run/7ed2a65e-1971-4040-9ce2-a88419f3ef2e) |
| 2 | pass | 100 | 18 | 19.6 | 3 | 3 | [run](https://argusic.com/run/1a0a3437-878d-41bb-bf1a-20f3bb53fcc4) |
| 3 | fail | 80 | 24 | 24.6 | 3 | 3 | [run](https://argusic.com/run/cc626a29-0a67-4490-b455-87751019f394) |

## What was observed on a clean machine

Attempt 2:

- 12 min: `Missing -dev packages for zlib, libpng, libjpeg, freetype, harfbuzz, libogg, libvorbis, openal, SDL2, libcurl, enet, bluez (no root access)`
- 1 min: `CMake FindZLIB could not find zlib headers/libs`
- 2 min: `libcurl found as static .a causing undefined refs to nghttp2, gssapi`
- 1 min: `curl/curl.h header not found (installed to multiarch path include/x86_64-linux-gnu/curl/)`
- 1 min: `libz.so symlink dangling (pointed to missing libz.so.1.3)`
- 1 min: `freetype2 and harfbuzz .pc files required libbrotlidec, glib-2.0, graphite2 (no .pc files)`

Attempt 2:

- 3 min: `Missing libz1g-dev, libpng-dev, libfreetype-dev, libharfbuzz-dev, libogg-dev, libvorbis-dev, libopenal-dev, libsdl2-dev, libcurl4-openssl-dev, libjpeg-turbo8-dev, libenet-dev, libsamplerate0-dev headers/libs (no root for apt install)`
- 2 min: `C++ operator!= not defined for ENetIP struct (bundled ENet uses struct-based address) in connect_to_server.cpp, socket_address.cpp, stk_host.cpp`
- 1 min: `Static libcurl.a missing nghttp2/gssapi link deps`

Attempt 3:

- 3 min: `Could NOT find ZLIB (missing: ZLIB_LIBRARY ZLIB_INCLUDE_DIR)`
- 2 min: `no match for operator!= (operand types are ENetIP and ENetIP)`
- 2 min: `undefined reference to nghttp2_* and gss_* functions from static libcurl.a`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
