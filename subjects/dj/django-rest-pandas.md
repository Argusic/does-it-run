# django-rest-pandas

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/wq/django-rest-pandas, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/django-rest-pandas

## Pinned environment

- Project commit: `7bdf912d16774133ce731100bf9a245917b0aa59`
- Test commit: `7bdf912d16774133ce731100bf9a245917b0aa59`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 5.2 to 7.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 7.9 | 4 | 4 | [run](https://argusic.com/run/6e7b83f3-3ceb-43d3-8ecd-1e88adc9df45) |
| 2 | pass | 100 | 4 | 5.2 | 4 | 4 | [run](https://argusic.com/run/1c0e7554-72b5-4325-9b11-ffaa377b84ec) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `pandas 3.0 Copy-on-Write broke fillna(inplace=True) causing NaN in index values, which cascaded into a TypeError in the scatter serializer`
- 1 min: `Missing Python deps: requests, matplotlib, django-pandas, itertable for test suite`
- 1 min: `Django runserver failed due to missing MIDDLEWARE and STATIC_URL trailing slash in test settings`
- 1 min: `@wq/chart had no built index.js so analyst tests couldn't resolve the jsx-charts dependency`

Attempt 2:

- 2 min: `Python package dependencies missing (requests, itertable not installed)`
- 8 min: `pandas 3.x incompatibility: inplace=True silently fails due to Copy-on-Write changes, fillna with string on float64 column raises TypeError`
- 5 min: `PandasScatterSerializer.transform_dataframe TypeError: unsupported operand type(s) for +: 'float' and 'str' when coord_names contain NaN after unstack`
- 1 min: `Django test settings missing MIDDLEWARE causing runserver system check failure on Django 6`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
