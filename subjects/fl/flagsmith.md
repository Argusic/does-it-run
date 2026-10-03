# flagsmith

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Flagsmith/flagsmith, licensed BSD-3-Clause, written in Python.

Evidence and recordings: https://argusic.com/subject/flagsmith

## Pinned environment

- Project commit: `78e3fd06ce43637b02bc55a0e465dc77b16ccedd`
- Test commit: `78e3fd06ce43637b02bc55a0e465dc77b16ccedd`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 39.8 to 87.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | n/a | 87.1 | 0 | 0 | [run](https://argusic.com/run/2aff8444-13bd-4e02-b5ca-57042fdf4620) |
| 2 | pass with mocks | 92 | 1.5 | 39.8 | 6 | 6 | [run](https://argusic.com/run/512777c4-37e0-45e3-b160-4b0277dcf9fa) |

## What was observed on a clean machine

Attempt 2:

- 5 min: `No Docker or PostgreSQL in container; API requires Postgres for full test suite`
- 3 min: `app_analytics migration 0007 uses RenameIndex which fails on SQLite (ValueError: wrong number of indexes)`
- 2 min: `app_analytics migration 0008 uses PostgreSQL DO block in RunSQL which fails on SQLite`
- 3 min: `ExperimentComputation(models.Model, Generic[SummaryT]) raises TypeError on Python 3.12: Cannot inherit from plain Generic`
- 2 min: `django.contrib.sites table missing with faked migrations; causes errors in helper tests`
- `npm run typecheck reports 6 TypeScript errors in frontend`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
