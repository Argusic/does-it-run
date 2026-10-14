# pywikibot

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/wikimedia/pywikibot, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/pywikibot

## Pinned environment

- Project commit: `ad6e1db6065316b4b66a94f68c9159bd50378de0`
- Test commit: `ad6e1db6065316b4b66a94f68c9159bd50378de0`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 9.5 to 9.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 9.5 | 3 | 3 | [run](https://argusic.com/run/7480be3f-f9ee-4884-858b-6f5f4547dc9a) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `pip install -r requirements.txt failed: externally-managed-environment (PEP 668 blocks system pip)`
- 1 min: `3 setup_tests failures: ModuleNotFoundError: No module named 'setuptools' in venv (setup.py get_packages)`
- 3 min: `5 doctest failures (Category.subcategories, BasePage.stable_revision, User.renamed_target, APISite.page_from_repository, TimeStripper) caused by live en.wikipedia.org HTTP 429 rate limiting and transient output lines`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
