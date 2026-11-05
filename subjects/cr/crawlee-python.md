# crawlee-python

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/apify/crawlee-python, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/crawlee-python

## Pinned environment

- Project commit: `45bb0e25df8fdad3caf0e756e32c2063717da4ce`
- Test commit: `45bb0e25df8fdad3caf0e756e32c2063717da4ce`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 7.5 to 35.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5.5 | 7.5 | 2 | 2 | [run](https://argusic.com/run/200f39e3-56d7-43b1-826d-c1e470ed4df5) |
| 2 | pass | 100 | 27 | 35.1 | 6 | 6 | [run](https://argusic.com/run/e49c02bf-b4b8-4957-ac66-ccbfe10911a2) |

## What was observed on a clean machine

Attempt 1:

- 0.3 min: `uv binary not in PATH after pip install to user site`
- 0.5 min: `Playwright Firefox browser not installed (only chromium was installed)`

Attempt 2:

- 2 min: `uv not installed; uv run poe install-dev unusable`
- 3 min: `Playwright install warned host system missing libs; cannot sudo install-deps`
- 5 min: `uv run poe install-dev exited 0 but unit-tests aborted with KeyboardInterrupt in pydantic SchemaValidator during pytest startup`
- 7 min: `pytest -n auto exits 137 with BrokenPipeError and 0 tests (TESTS_CONCURRENCY=auto)`
- 18 min: `PlaywrightCrawler with Configuration(disable_browser_sandbox=True) ignored the setting; Chromium died with 'No usable sandbox!' SIGTRAP`
- 8 min: `mid-fix attempt syncing global service_locator broke test_passing_configuration with ServiceConflictError`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
