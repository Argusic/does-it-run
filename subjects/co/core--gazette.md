# core

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/gazette/core, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/run/5b2aee7a-ada5-4cfd-ab84-1b144063b958

## Pinned environment

- Project commit: `fc6a39822be652c67b13842b9cd760e80d7d6731`
- Test commit: `fc6a39822be652c67b13842b9cd760e80d7d6731`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 37 to 37 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 35 | 37 | 4 | 4 | [run](https://argusic.com/run/5b2aee7a-ada5-4cfd-ab84-1b144063b958) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `go: not found (no Go toolchain in container)`
- 2 min: `exec: 'etcd': executable file not found in $PATH (tests spawn real etcd)`
- 15 min: `consumer/store-rocksdb and consumer/store-sqlite (and examples) fail: rocksdb/c.h: No such file or directory; pinned jgraettinger/gorocksdb C API no longer matches current RocksDB headers`
- 8 min: `libsqlite3.a static link undefined references to libm symbols (log/sin/sqrt etc)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
