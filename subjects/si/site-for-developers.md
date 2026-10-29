# site-for-developers

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/currenjin/site-for-developers, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/site-for-developers

## Pinned environment

- Project commit: `cac25bc2c1ad96fefebcfe0f7dd29d1770d1acee`
- Test commit: `cac25bc2c1ad96fefebcfe0f7dd29d1770d1acee`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 6.2 to 6.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8 | 6.2 | 3 | 3 | [run](https://argusic.com/run/2fd686e8-7a7b-4aba-a455-abf01e66fa13) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `System Python externally managed (PEP 668) blocked 'pip install playwright==1.58.0'`
- 3 min: `Playwright not installed so browser test modules (test_site_browser, test_locale_browser, test_static_seo) failed to import`
- 2 min: `'playwright install chromium' reported exit code 2 with '/bin/sh: 1: Bad substitution' due to the container's login-shell profile`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
