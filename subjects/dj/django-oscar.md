# django-oscar

**Verdict: runs.** Argusic Score 90 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/django-oscar/django-oscar, licensed BSD-3-Clause, written in Python.

Evidence and recordings: https://argusic.com/subject/django-oscar

## Pinned environment

- Project commit: `076197f4ccd5e1785dbbdf99075d601b3d510c7d`
- Test commit: `076197f4ccd5e1785dbbdf99075d601b3d510c7d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 8.3 to 11.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 80 | 11 | 11.3 | 4 | 0 | [run](https://argusic.com/run/e90a6b14-ae68-4a7b-a9be-3ea807dbcad0) |
| 2 | pass | 100 | 0.5 | 8.3 | 3 | 3 | [run](https://argusic.com/run/79dc098f-73ef-4c99-9016-cbc4740c6a30) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `test_updating_subtree_slugs_when_moving_category_to_new_parent: Category.full_slug cache polluted by prior test with same PK on SQLite`
- 5 min: `test_updating_subtree_when_moving_category_to_new_sibling: same root cause`
- 5 min: `test_single_usage: SQLite cannot handle concurrent writes for concurrency test`
- 5 min: `test_voucher_single_usage: same root cause`

Attempt 2:

- 0.5 min: `System pip blocked by externally-managed-environment (PEP 668)`
- `2 category tests fail due to locmem cache pollution across test cases`
- `2 concurrent order placement tests fail with SQLite 'database table is locked'`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
