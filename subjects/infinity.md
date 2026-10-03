# infinity

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/infiniflow/infinity, licensed Apache-2.0, written in C++.

Evidence and recordings: https://argusic.com/subject/infinity

## Pinned environment

- Project commit: `b1083912a5002c72207a9ed37c4b0957f21b4f35`
- Test commit: `b1083912a5002c72207a9ed37c4b0957f21b4f35`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 12.4 to 82.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | 72 | 82.9 | 3 | 3 | [run](https://argusic.com/run/993ac8e1-e647-452a-b7ac-f2ae838a2adb) |
| 2 | pass | 100 | 8 | 12.4 | 3 | 3 | [run](https://argusic.com/run/51440e1e-710b-4d2e-b4b8-ccbab68f2ef8) |

## What was observed on a clean machine

Attempt 1:

- 40 min: `vcpkg build of arrow+parquet (273 source files) did not complete within time budget (~40 min on 4-core)`
- 15 min: `11 remaining vcpkg deps not installed: nlohmann-json, pcre2, spdlog, simdjson, magic-enum, oatpp, pugixml, roaring, rocksdb, simde, parallel-hashmap, jemalloc, vit-vit-ctpl`
- 10 min: `Python datrie package failed to build from source (missing Python.h)`

Attempt 2:

- 2 min: `Cannot build from source: container lacks clang-20, cmake 4.x, vcpkg, and root apt access`
- 2 min: `Cannot create /var/infinity and /usr/share/infinity/resource - no root`
- `Can not pin thread! warnings printed at startup`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
