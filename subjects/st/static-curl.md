# static-curl

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/stunnel/static-curl, licensed MIT, written in Shell.

Evidence and recordings: https://argusic.com/subject/static-curl

## Pinned environment

- Project commit: `22338b1f21b80a9705299770b487ab2224cff92e`
- Test commit: `22338b1f21b80a9705299770b487ab2224cff92e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 53.6 to 89.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | 76 | 89.5 | 3 | 2 | [run](https://argusic.com/run/cbb07716-90c1-4d04-8fd0-5a22285f7c58) |
| 2 | pass | 100 | 46 | 53.6 | 5 | 5 | [run](https://argusic.com/run/929be239-46fb-45bb-abb2-350d2f1a84ca) |

## What was observed on a clean machine

Attempt 1:

- 15 min: `No Docker CLI in this unprivileged container; the script's Docker fallback would fail silently and the bare install command dies on root-only apt and /mnt writes`
- 25 min: `Native x86_64 builds hard-select clang-20; this container has no clang and no root to install it, so OpenSSL make fails with clang-20 not found`
- 36 min: `Non-root container lacks wget, autoreconf/autoconf, and apt write access; libpsl 0.23.3 tarball has no configure and libunistring needs autoreconf, so the static build stops there after OpenSSL/zlib/zstd/libidn2/libunistring built`

Attempt 2:

- 8 min: `README standard path 'sh curl-static-cross.sh' requires Docker (missing) and apt/root (no sudo, apt lock Permission denied)`
- 12 min: `wget was not installed and the script's download step needs a wget with HTTPS (wget built without TLS refused 'wget https://...' with 'HTTPS support not compiled in')`
- 9 min: `The script hardcodes clang/clang-20 (apt metadata) but no clang exists in the container; clang-20 not found aborted OpenSSL and CXX=clang++-20 aborted zstd CMake`
- 10 min: `autotools (m4, autoconf, automake, libtool/autoreconf) and makeinfo were missing; libpsl configure died on PKG_PROG_PKG_CONFIG (pkg.m4) and curl's autoreconf needs the full stack`
- `curl's own test suite failed 19 tests, all IPv6 tests`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
