# neon

**Verdict: could not verify.** Argusic Score 20 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/neondatabase/neon, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/neon

## Pinned environment

- Project commit: `fa504217c61bbcaf5c512d75830564541f917f8f`
- Test commit: `fa504217c61bbcaf5c512d75830564541f917f8f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, no run possible
- Valid runs: 2; wall time 64.9 to 92.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | 91 | 92.6 | 15 | 15 | [run](https://argusic.com/run/59b24a30-586e-4cbe-a843-cfe27b3d3500) |
| 2 | fail | 20 | n/a | 64.9 | 0 | 0 | [run](https://argusic.com/run/3873d80d-cb70-42fe-90b3-1295bd8a80a0) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `protoc not found - required for protobuf compilation`
- 1 min: `protoc include files missing (google/protobuf/*.proto)`
- 10 min: `libclang not found - required by bindgen for postgres_ffi`
- 8 min: `clang builtin headers (stddef.h etc) missing - bindgen could not find them`
- 5 min: `neon-pg-ext build failed: libcurl headers and library missing`
- 1 min: `neon-pg-ext build failed: libpq-events.h not found (wrong include path)`
- 2 min: `Linker OOM on storage_scrubber binary`
- 1 min: `endpoint_storage binary not built initially`
- 1 min: `PostgreSQL v17 submodule not initialized`
- 3 min: `PostgreSQL configure failed: bison, flex, m4 not found`
- 4 min: `PostgreSQL configure failed: ICU library not found (missing .pc files and headers)`
- 1 min: `PostgreSQL configure failed: readline library not found`
- 1 min: `PostgreSQL configure failed: zlib not found and libseccomp not found`
- 3 min: `PostgreSQL link failed: static ICU libs need C++ link flags`
- 1 min: `neon_local start failed initially because endpoint_storage binary missing`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
