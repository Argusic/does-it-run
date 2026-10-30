# aurora

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/capjamesg/aurora, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/aurora

## Pinned environment

- Project commit: `2a9aae47996ba1ac75b3b5c49646f470a878bf5a`
- Test commit: `2a9aae47996ba1ac75b3b5c49646f470a878bf5a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 5.3 to 5.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 7 | 5.3 | 7 | 7 | [run](https://argusic.com/run/aedb287e-b5e2-4abd-8995-839b4c061de4) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `pip3 install -e . failed: externally-managed-environment (PEP 668)`
- 1 min: `pytest tests/ failed with No module named pytest; no test_*.py files exist, tests are in tests/state.py`
- 4 min: `7 of 19 tests failed: OS error 2 FileNotFoundError from is_safe_path in every build`
- 3 min: `Data collection pages missing: CSV files never discovered and all JSON records written to <collection>/index.html`
- 1 min: `test_new_site_generation failed: sh: aurora: not found`
- 2 min: `Archive tests failed without SITE_ENV; fixtures assume production base URL`
- 2 min: `aurora build docs failed: bs4 FeatureNotFound lxml`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
