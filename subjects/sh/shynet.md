# shynet

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/milesmcc/shynet, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/shynet

## Pinned environment

- Project commit: `ca35caba3af2b888acc990b99152c500a1c44461`
- Test commit: `ca35caba3af2b888acc990b99152c500a1c44461`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 6.3 to 19.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 20 | 19.9 | 5 | 5 | [run](https://argusic.com/run/7c902703-7e38-482b-a26b-882a8ea36b09) |
| 2 | pass | 100 | 7 | 6.3 | 4 | 4 | [run](https://argusic.com/run/5a3959ad-d85e-40a6-a5b1-d17e111bcada) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `No C compiler available. Dependencies frozenlist, multidict, cffi required native compilation which failed.`
- 1 min: `django-allauth 0.63.6 requires AccountMiddleware to be added to MIDDLEWARE settings.`
- 1 min: `NPM_ROOT_PATH was set to '../' which resolved to /work (parent of shynet/) instead of /work/repo/node_modules.`
- 2 min: `Staticfiles manifest missing: whitenoise CompressedManifestStaticFilesStorage requires a manifest file.`
- 1 min: `STATICFILES_DIRS was empty, preventing static file collection from node_modules.`

Attempt 2:

- 2 min: `poetry install failed building frozenlist 1.3.1 and multidict 6.0.2 from source (missing python3-dev headers)`
- 1 min: `django-health-check v4 removed health_check.db and health_check.cache submodules that Shynet INSTALLED_APPS requires`
- 1 min: `allauth.account.middleware.AccountMiddleware not in MIDDLEWARE (required by django-allauth 65.x)`
- 1 min: `collectstatic failed because NPM_ROOT_PATH='../' resolved to /work instead of /work/repo`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
