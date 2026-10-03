# OHMySQL

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/oleghnidets/OHMySQL, licensed MIT, written in C.

Evidence and recordings: https://argusic.com/subject/ohmysql

## Pinned environment

- Project commit: `cc1874ddaaa8a1fddf24c0fa399d928867b7eca2`
- Test commit: `cc1874ddaaa8a1fddf24c0fa399d928867b7eca2`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 28.5 to 70.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | 30 | 28.5 | 9 | 9 | [run](https://argusic.com/run/af4dd86b-6384-45f1-b91d-f1cce0fe91d5) |
| 2 | pass | 100 | 58 | 70.5 | 7 | 7 | [run](https://argusic.com/run/6dc2c564-9e66-43c3-9882-f8ced559d1ac) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Swift compiler not found on Ubuntu 24.04`
- 1 min: `libncurses.so.6 missing for Swift binary`
- 5 min: `MySQL server binary and dependencies not available`
- 2 min: `MySQL server failed to start: need --secure-file-priv directory`
- 3 min: `MySQL server crashed after brief startup (process check timeout)`
- 2 min: `MySQL client failing with 'Connection refused' via both socket and TCP`
- 5 min: `Apple xcframework binaries (MySQL.xcframework, OpenSSL.xcframework) are Mach-O format (cafebabe header) and cannot link on Linux`
- 5 min: `Objective-C source files require Foundation/ObjC runtime, which Swift on Linux clang lacks`
- 2 min: `OHMySQL Package.swift declares binary targets for xcframeworks that do not exist on Linux`

Attempt 2:

- 30 min: `Original framework is iOS/macOS ObjC with Apple XCFrameworks - cannot build natively on Linux`
- 5 min: `Swift 6.0 toolchain missing on Linux - libncurses.so.6 not found`
- 10 min: `MySQL server needed for tests - not installed`
- 5 min: `MariaDB client could not load caching_sha2_password auth plugin`
- 3 min: `NSObject KVC (setValue:forKeyPath:) not available on Linux Foundation`
- 3 min: `Connection tests hung due to deadlock in MySQLStoreCoordinator reconnect`
- 2 min: `ObjC interop disabled on Linux - @objc attributes fail`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
