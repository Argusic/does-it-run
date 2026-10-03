# warzone2100

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Warzone2100/warzone2100, licensed GPL-2.0, written in C++.

Evidence and recordings: https://argusic.com/subject/warzone2100

## Pinned environment

- Project commit: `549de5860df0fbfae19b3ca8dddd239ff032770b`
- Test commit: `549de5860df0fbfae19b3ca8dddd239ff032770b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 3; wall time 42 to 75.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | n/a | 42 | 0 | 0 | [run](https://argusic.com/run/f9fb22a9-e769-4e9f-bc67-1ff0f1f7f8c0) |
| 1 | pass | 100 | 78 | 75.3 | 7 | 7 | [run](https://argusic.com/run/9a0543c9-b996-45e5-966e-29e842cd8c58) |
| 2 | timeout | none | n/a | 42 | 0 | 0 | [run](https://argusic.com/run/d00e990a-ecaa-4499-af9a-3b458fd77f7a) |

## What was observed on a clean machine

Attempt 1:

- 15 min: `Missing system -dev packages (no root access). Downloaded .deb packages and extracted to a local sysroot.`
- 8 min: `Git submodules not initialized (3rdparty deps + data files needed)`
- 12 min: `SDL3 not available on Ubuntu 24.04 (requires SDL3 >= 3.2.12)`
- 5 min: `CMake configuration failures due to missing submodules (utf8proc, launchinfo, fmt, re2, fonts, ControllerImage, terrain_overrides, campaign data)`
- 1 min: `libzip CMake config references missing zipcmp/zipmerge/ziptool executables`
- 10 min: `Missing runtime .so versioned files for curl dependencies (brotli, nghttp2, nettle, hogweed, gmp, gnutls, unistring, gssapi_krb5, lber, ldap, ssh, psl, sasl2, ssl)`
- 5 min: `Static linking of libcurl.a causes endless dependency chain of private libs (needing gssapi_krb5, lber, ldap, sasl2, ssl, crypto, pq, mysql)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
