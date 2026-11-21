# pghoard

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Aiven-Open/pghoard, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/pghoard

## Pinned environment

- Project commit: `a531b8efc05addaba66a8525c383a6998f156546`
- Test commit: `a531b8efc05addaba66a8525c383a6998f156546`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 11.1 to 47.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 45 | 47.8 | 4 | 4 | [run](https://argusic.com/run/fcc28e1d-9a52-447f-be6d-78f27852d0f1) |
| 2 | pass with mocks | 92 | 0.7 | 11.1 | 3 | 3 | [run](https://argusic.com/run/0a19eabc-a76f-4a55-bd7a-9cf409647b74) |

## What was observed on a clean machine

Attempt 1:

- `test_graceful_shutdown: assert 0 - Python 3.12 mock_open compatibility issue`
- `test_pause_on_disk_full: needs sudo for tmpfs mount`
- `IPv6 tests (4): no IPv6 support in container`
- `test_basebackups_tablespaces: PostgreSQL restore fails - pghoard_postgres_command not found`

Attempt 2:

- `No PostgreSQL binaries installed - 196 parametrized tests requiring 'db' fixture (real PG server) skipped with RuntimeError`
- `'test_pghoard.py::test_graceful_shutdown' fails on Race condition: assertion qsize==0 fails because slow_compress file-not-found errors`
- `Pydantic V2 deprecation warnings for '.parse_raw', '.json()', 'parse_raw'; datetime.datetime.utcnow() deprecation`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
