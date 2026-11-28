# Xapiand

**Verdict: could not verify.** Argusic Score 17.5 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Kronuz/Xapiand, licensed MIT, written in C++.

Evidence and recordings: https://argusic.com/subject/xapiand

## Pinned environment

- Project commit: `b7e673ab601ffc75ad09d4ca5e532ba583e2151f`
- Test commit: `b7e673ab601ffc75ad09d4ca5e532ba583e2151f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 2; wall time 35.6 to 51.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | 45 | 35.6 | 5 | 5 | [run](https://argusic.com/run/08ab99e8-b0dc-4fef-a221-65b096ff833f) |
| 2 | fail | 15 | 42 | 51.1 | 12 | 9 | [run](https://argusic.com/run/79ad5b13-d861-4a39-9d53-75fcb20e8938) |

## What was observed on a clean machine

Attempt 1:

- 10 min: `uuid-dev, zlib1g-dev, libzstd-dev, libtcl8.6, libicu-dev not installed (no root)`
- 5 min: `threadpool renamed to workpool causing target conflict`
- 10 min: `MsgPack/cuuid renamed serialise to serialize`
- 5 min: `storage::posix not declared in fetched storage dependency`
- 15 min: `All 60+ deps pinned to main with incompatible API changes`

Attempt 2:

- 7 min: `Missing system -dev packages: uuid-dev, zlib1g-dev, libzstd-dev (could not install via apt, no root). Manually extracted headers/libs from Ubuntu .deb packages via curl+dpkg -x.`
- 5 min: `Missing tclsh for Xapian Unicode data generation. Installed tcl8.6 binary + libtcl8.6 from Debian packages.`
- 3 min: `CMake target collision: threadpool repo (Kronuz/threadpool) and workpool repo (Kronuz/workpool) both define 'workpool' target. Changed FetchContent_MakeAvailable(threadpool) to FetchContent_Populate(threadpool) to avoid building the threadp`
- 2 min: `Missing wheel.hh include: logger.h includes wheel.hh from Kronuz/wheel, which wasn't included in main include path. Added FetchContent for wheel library.`
- 6 min: `MsgPack::serialise/unserialise API renamed to serialize/unserialize (American spelling) in the Kronuz/msgpack library. Fixed 18 call sites.`
- 1 min: `cuuid::serialise renamed to serialize. Fixed 2 call sites.`
- 1 min: `UUID::is_serialised renamed to is_serialized. Fixed 2 call sites.`
- 3 min: `storage::posix namespace missing from xapiand_storage_io.h (which replaces storage_io.h entirely). Added posix lock/truncate helpers to xapiand_storage_io.h.`
- 1 min: `xapiand_storage_trace.h included logger.h (doesn't exist), should include log.h.`
- 5 min: `reactor::PeriodicTimer was removed from main branch of the reactor library. cluster library uses it. Pinned reactor to ab69cf2, but FetchContent caching caused stale fetch. Also PeriodicTimer removed from reactor between pin and the fetched`
- 2 min: `http::Request API changed: body_reader() doesn't exist (probably renamed). + HttpAsioService constructor changed signature. + SearchService override signatures don't match base.`
- 6 min: `19 remaining compile errors after ~42 min of fixing; root cause is that all 59+ Kronuz/* dependencies track 'main' branch which has diverged from what this repo's source expects.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
