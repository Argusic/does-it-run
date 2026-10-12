# Mastodon.py

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/halcy/Mastodon.py, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/mastodon-py

## Pinned environment

- Project commit: `b9f2effbb5a9f07ebca3807466f4130e69b1614c`
- Test commit: `b9f2effbb5a9f07ebca3807466f4130e69b1614c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 11 to 11 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 1 | 11 | 2 | 2 | [run](https://argusic.com/run/29ea093b-753b-4ae5-84db-f2a0eb9ca5bb) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `System pip install rejected by PEP 668 externally-managed-environment`
- 2 min: `test_status_length failed: get_status_length raised NotImplementedError because optional grapheme module was not installed (tests README omits the extra that tox.ini lists)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
