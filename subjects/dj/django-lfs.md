# django-lfs

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/diefenbach/django-lfs, licensed BSD-3-Clause, written in Python.

Evidence and recordings: https://argusic.com/subject/django-lfs

## Pinned environment

- Project commit: `3385b9a583abfaf8c9043cc669432051b957edac`
- Test commit: `3385b9a583abfaf8c9043cc669432051b957edac`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 18.6 to 18.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 18.6 | 7 | 7 | [run](https://argusic.com/run/e9ab1792-1765-428f-995e-3070be40e303) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `ugettext_lazy removed in Django 6 - 7 third-party packages affected`
- 2 min: `ForeignKey missing on_delete in 5 dependency packages`
- 1 min: `django.core.urlresolvers removed in Django 4+`
- 1 min: `django.conf.urls.url removed in Django 5+`
- 3 min: `Missing Python dependencies`
- 0.5 min: `Migration dependency broken reference`
- 1 min: `Django settings missing required LFS config values`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
