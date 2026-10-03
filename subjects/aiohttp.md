# aiohttp

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/aio-libs/aiohttp, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/aiohttp

## Pinned environment

- Project commit: `60bffb410dcdd46ec96d843854edec44e8c05557`
- Test commit: `60bffb410dcdd46ec96d843854edec44e8c05557`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 14 to 14 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 14 | 6 | 6 | [run](https://argusic.com/run/53427ea4-8d8e-4775-9b61-b00a216af5f3) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `externally-managed-environment blocks system pip install`
- 0.5 min: `git submodules not initialized`
- 1 min: `Cython .c files missing (mask, reader_c, _http_writer, _find_header)`
- 1 min: `pytest_cov and pytest_aiohttp plugins not found`
- 0.5 min: `ModuleNotFoundError for Brotli and gunicorn in test suite`
- 2 min: `test_body_part_reader_payload_write fails: mock.create_autospec(write=write, spec_set=True) ignores the write kwarg in Python 3.12`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
