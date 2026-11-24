# paozhu

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/hggq/paozhu, licensed MIT, written in C++.

Evidence and recordings: https://argusic.com/subject/paozhu

## Pinned environment

- Project commit: `a6094e298dab2f5191e47b7dd6fd89f156590406`
- Test commit: `a6094e298dab2f5191e47b7dd6fd89f156590406`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 17.6 to 27 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 55 | 17.6 | 5 | 5 | [run](https://argusic.com/run/7e592936-2198-47c9-9b1c-9ed2d443c456) |
| 2 | pass | 100 | 26 | 27 | 5 | 5 | [run](https://argusic.com/run/ea7b0231-7774-45fc-b88a-9c83b5d2b1a9) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Missing Asio standalone headers (asio.zip not extracted)`
- 5 min: `Brotli headers not found (brotli/encode.h)`
- 3 min: `Brotli static link: undefined references to _kBrotliPrefixCodeRanges etc.`
- 2 min: `cmake file(MAKE_DIRECTORY /usr/local/etc/paozhu) fails with Permission denied`
- 10 min: `Missing zlib/brotli/sqlite3 -dev headers`

Attempt 2:

- 10 min: `Missing development headers: zlib1g-dev (zlib.h, libz.so symlink), libbrotli-dev (brotli/encode.h), libsqlite3-dev (sqlite3.h)`
- 3 min: `Asio zip extraction created 3-level nesting (asio/asio/asio/*.hpp) but asio.hpp at root expects includes as asio/*.hpp`
- 2 min: `libbrotlienc.so and libbrotlidec.so had only .so.1 symlinks, no .so symlink for find_library`
- 1 min: `libz.so symlink missing from system (only libz.so.1 and libz.so.1.3 present)`
- 1 min: `Release build fails because CMakeLists.txt tries to copy configs to /usr/local/etc/ (no root)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
