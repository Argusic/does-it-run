# saleor

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/saleor/saleor, licensed BSD-3-Clause, written in Python.

Evidence and recordings: https://argusic.com/subject/saleor

## Pinned environment

- Project commit: `5ff56489737c78a9a5631d528f699303c953696a`
- Test commit: `5ff56489737c78a9a5631d528f699303c953696a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 42.3 to 42.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 40 | 42.3 | 3 | 3 | [run](https://argusic.com/run/107270ed-1f55-4bf2-9446-8f6a9631b886) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `libmagic.so not found - python-magic ImportError on startup`
- 5 min: `pywatchman dev dependency fails to compile - no python3.12-dev headers`
- 10 min: `SQLite incompatible - Saleor requires PostgreSQL (django.contrib.postgres)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
