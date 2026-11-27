# osrm-backend

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Project-OSRM/osrm-backend, licensed BSD-2-Clause, written in C++.

Evidence and recordings: https://argusic.com/subject/osrm-backend

## Pinned environment

- Project commit: `454d73a96826fd1d94c474a3f2f8304ddc7c62ad`
- Test commit: `454d73a96826fd1d94c474a3f2f8304ddc7c62ad`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 52.7 to 52.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 52 | 52.7 | 8 | 8 | [run](https://argusic.com/run/0a4ec2cc-6c94-4ef5-9091-5ff442f88bef) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Missing zip/unzip tools for vcpkg binary caching`
- 3 min: `System CMake 3.28 too old (needs CMP0156 policy from CMake 4.x)`
- 2 min: `vcpkg bootstrap needs zip which is not installed`
- 1 min: `No ninja build system installed`
- 2 min: `Osmium header missing '#include <cassert>' (Werror breaks build)`
- 2 min: `Lua deb ships lua5.4-deb-multiarch.h in arch-specific path, not found by compiler`
- 10 min: `Static libarchive.a needs OpenSSL/BZip2/Zstd/ZLib/LZMA transitive link deps`
- 5 min: `TBB and Lua5.4 .a/.so files missing from vcpkg partial install`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
