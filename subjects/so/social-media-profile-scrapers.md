# social-media-profile-scrapers

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/shaikhsajid1111/social-media-profile-scrapers, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/social-media-profile-scrapers

## Pinned environment

- Project commit: `ced2abf4f6974e0972f71a81d74610a37a31d9b7`
- Test commit: `ced2abf4f6974e0972f71a81d74610a37a31d9b7`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 15.8 to 15.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 15.8 | 8 | 8 | [run](https://argusic.com/run/da469057-7516-4486-86dc-2523cd3f3359) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `PEP 668 externally-managed environment blocked system pip install`
- 6 min: `All 8 tests failed: tests.py asserts scrapers return dict, but refactored scrapers return JSON string; Twitter.scrap() and Medium.scrap() take 1 arg (not 2); Reddit/Quora use deprecated Selenium executable_path kwarg from webdriver_manager;`
- 3 min: `Facebook curl_cffi redirected to www.facebook.com React shell (validator rejects it); seleniumbase_uc UC browser back-end fails with I/O operation on closed file`
- 1 min: `Instagram API returns HTTP 429 without real session cookies`
- 1 min: `Twitter guest token API changed (no guest_token in response)`
- 1 min: `Medium GraphQL endpoint returns nothing for test user`
- 1 min: `No Chrome or Firefox browser binary found on PATH; Quora and Reddit scrapers hang trying to start Selenium browsers`
- 1 min: `webdriver_manager not installed (imported by Reddit/Quora)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
