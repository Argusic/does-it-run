# vearch

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/vearch/vearch, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/vearch

## Pinned environment

- Project commit: `bae78b189ff0ab1d8ac659c6acaeeb5f630db33f`
- Test commit: `bae78b189ff0ab1d8ac659c6acaeeb5f630db33f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 15.1 to 59 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 90 | 59 | 6 | 6 | [run](https://argusic.com/run/4af1780f-c0d0-4167-81f7-b0d900544e7c) |
| 2 | pass with mocks | 92 | 35 | 15.1 | 3 | 3 | [run](https://argusic.com/run/ff7d5616-0dfc-4eef-a88d-f473f2d401fc) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `No Go compiler on system`
- 10 min: `Missing system C++ libs (OpenBLAS, TBB, protobuf, roaring, rocksdb, zstd)`
- 10 min: `Ubuntu CRoaring v0.2.66 lacks C++ namespace (roaring::Roaring64Map), headers incompatible with gamma engine`
- 20 min: `pip faiss-cpu ABI mismatch with gamma engine linking`
- 5 min: `Static libs (rocksdb.a, zstd.a) incompatible with -fPIC shared lib linking`
- 10 min: `PS heartbeat drops causing server unavailability in tests`

Attempt 2:

- 2 min: `Go 1.22 not pre-installed`
- 5 min: `Gamma C++ engine dependencies (protobuf, rocksdb, CRoaring, faiss, DiskANN, MKL) not available and cannot be built without root`
- 3 min: `Stale etcd WAL data from previous runs caused etcd startup failure`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
