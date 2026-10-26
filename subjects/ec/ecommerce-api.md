# ecommerce_api

**Verdict: could not verify.** Argusic Score 50 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/thomas545/ecommerce_api, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/ecommerce-api

## Pinned environment

- Project commit: `ce65724cf3ca9ef42a7f58be772602fc9b131a8a`
- Test commit: `ce65724cf3ca9ef42a7f58be772602fc9b131a8a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 2; wall time 13 to 48.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 47 | 48.2 | 24 | 24 | [run](https://argusic.com/run/1c36f160-4dee-41c3-94f1-4f4310c667c2) |
| 2 | fail | 20 | n/a | 13 | 0 | 0 | [run](https://argusic.com/run/473839e6-77dd-49d0-a909-c7d55b433476) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `clyent==1.2.2 not found on PyPI`
- 1 min: `pyodbc===4.0.0-unsupported malformed pin`
- 1 min: `install==1.3.5 not found`
- 5 min: `mysqlclient==2.2.6 has no x86_64 Linux wheel and build fails without mysql headers`
- 1 min: `psycopg2==2.9.10 source build needs libpq-dev`
- 2 min: `Windows-only packages uninstallable (pywin32, comtypes, pyreadline, etc.)`
- 1 min: `ruamel-yaml-conda build fails`
- 1 min: `fastcache, pycosat, typed-ast sdist build fails`
- 1 min: `pywinpty needs maturin build backend`
- 1 min: `twisted-iocpsupport build fails`
- 3 min: `django-haystack version metadata broken on PyPI; pip reports '0.0.0'`
- 5 min: `PyJWT version conflict: djangorestframework-jwt requires <2.0, firebase-admin requires >=2.5`
- 3 min: `ugettext/ugettext_lazy removed in Django 5.x`
- 1 min: `Signal(providing_args=...) removed in Django 5.x`
- 2 min: `Jet admin theme incompatible with Django 5 (python_2_unicode_compatible, django.conf.urls.url)`
- 1 min: `allauth.account.middleware.AccountMiddleware required`
- 2 min: `smart_text/force_text removed from django.utils.encoding`
- 1 min: `Memcached backend class renamed`
- 1 min: `Missing redis, pymemcache packages`
- 1 min: `elastic-transport version too new`
- 1 min: `elasticsearch-dsl 8.x incompatible with django-elasticsearch-dsl-drf`
- 1 min: `googletrans uses removed httpcore.SyncHTTPTransport type`
- 1 min: `rest_auth uses removed django.conf.urls.url`
- 2 min: `allauth.utils missing email_address_exists and get_username_max_length`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
