# UStore

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/unum-cloud/UStore, licensed Apache-2.0, written in C++.

Evidence and recordings: https://argusic.com/subject/ustore

## Pinned environment

- Project commit: `64b1256117cc2a154680f1bdf812d9dc6fc0ec77`
- Test commit: `64b1256117cc2a154680f1bdf812d9dc6fc0ec77`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 23 to 35.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | 0 | 23 | 2 | 2 | [run](https://argusic.com/run/91cfc884-fcfc-4134-bc95-458d4715d3fb) |
| 2 | pass | 100 | 28 | 35.8 | 6 | 6 | [run](https://argusic.com/run/4fa17010-ad67-4ad6-ac62-fc3ebcfdd194) |

## What was observed on a clean machine

Attempt 1:

- 45 min: `Native C++ build is impossible without root (no system packages) and without prebuilt Conan dependency archives from the private 'ustore-deps' GitHub repo`
- `test_merge (table_test.py) fails: pyarrow version incompatibility - pa.RecordBatch.from_pandas() in pyarrow 26 produces 'large_string' type, while the C++ bindings would produce 'string' type. Test was designed for pyarrow 10.x`

Attempt 2:

- 12 min: `MPack dependency from private unum-cloud/mpack repo not accessible`
- 3 min: `Python 3.12 development headers not installed`
- 8 min: `RocksDB 6.29.5 doesn't compile with GCC 13 (missing cstdint, system_error)`
- 1 min: `Missing cstdint include in include/ustore/cpp/types.hpp`
- 5 min: `UCSet engine from restructured public repo missing consistent_set.hpp`
- 2 min: `Arrow 19 API change in parquet::arrow::FileWriter::Open`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
