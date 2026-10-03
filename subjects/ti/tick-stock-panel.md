# tick-stock-panel

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/shy3130/tick-stock-panel, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/tick-stock-panel

## Pinned environment

- Project commit: `bab609b2d42c4722d51260a6c2192bbf16ab9139`
- Test commit: `bab609b2d42c4722d51260a6c2192bbf16ab9139`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 3; wall time 9.9 to 24 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3.5 | 9.9 | 0 | 0 | [run](https://argusic.com/run/357b2b12-a42f-4867-8504-5e2552ee74af) |
| 2 | pass | 100 | 10 | 10.7 | 1 | 1 | [run](https://argusic.com/run/45f0228b-84ba-4fb2-82c3-2208db45e503) |
| 3 | pass | 100 | 3 | 24 | 3 | 3 | [run](https://argusic.com/run/a00f2e50-88ea-4083-910f-b0ec4306c816) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `Flaky test failure in test_ext_config_load_all_cache.py::test_upsert_edit_invalidates_cache , passes when run individually but fails under full suite ordering`

Attempt 3:

- 2 min: `test_benchmark_momentum_today_excludes_today_rows: UTC date.today() vs CN_TZ offset caused today filter mismatch (pipeline uses CN_TZ, test used UTC)`
- 3 min: `test_pipeline_self_heals_snapshot_day: same UTC vs CN_TZ discrepancy , test's CN_TZ today was 2026-09-25 but pipeline's internal date.today() was 2026-09-24, so snapshot partition was treated as 'today' and skipped`
- 1 min: `test_upsert_edit_invalidates_cache: ExtConfigStore.upsert didn't invalidate _load_all_cache, so load_all returned stale data when mtime_ns didn't change between writes`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
