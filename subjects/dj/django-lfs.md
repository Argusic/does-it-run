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
- Valid runs: 2; wall time 18.6 to 60.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 18.6 | 7 | 7 | [run](https://argusic.com/run/e9ab1792-1765-428f-995e-3070be40e303) |
| 2 | pass | 100 | 10 | 60.6 | 11 | 11 | [run](https://argusic.com/run/bc039c96-f3aa-4bca-a02a-d79c4595dca6) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `ugettext_lazy removed in Django 6 - 7 third-party packages affected`
- 2 min: `ForeignKey missing on_delete in 5 dependency packages`
- 1 min: `django.core.urlresolvers removed in Django 4+`
- 1 min: `django.conf.urls.url removed in Django 5+`
- 3 min: `Missing Python dependencies`
- 0.5 min: `Migration dependency broken reference`
- 1 min: `Django settings missing required LFS config values`

Attempt 2:

- 3 min: `Django 6.x removed ugettext_lazy; patched portlets, reviews, postal`
- 4 min: `Django 6.x requires explicit on_delete on ForeignKey fields`
- 1 min: `Django 6.x requires ModelForm must declare fields`
- 3 min: `Missing dependencies (Pillow, Babel, django-reviews, django-postal, django-localflavor, captcha, crispy-forms, compressor)`
- 1 min: `lfs_contact.urls module not present`
- 2 min: `No Django project settings existed`
- 1 min: `No ROOT_URLCONF existed including manage URLs`
- 1 min: `Template contains {% load sql %} with no matching library`
- 1 min: `Shipping calculator dotted path wrong in settings`
- 1 min: `portlets.example app has no migrations`
- 1 min: `django-postal postal/forms/__init__.py dict_items type error`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
