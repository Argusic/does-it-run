# csp

**Verdict: runs.** Argusic Score 93.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Point72/csp, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/csp

## Pinned environment

- Project commit: `4247a8b581d5052e13eb97022d94aaaebe44b872`
- Test commit: `4247a8b581d5052e13eb97022d94aaaebe44b872`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 37.9 to 37.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 93.33 | 2.5 | 37.9 | 6 | 4 | [run](https://argusic.com/run/29db2a1b-d40d-45f5-bae9-929d251a418f) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Source build failed: missing python3-dev headers (Development.Embed component not found)`
- `Source build failed: vcpkg dependency tree incomplete - arrow, parquet, thrift, librdkafka, gtest not fully installed`
- `test_examples.py collection error: examples directory not bundled in PyPI wheel`
- 1 min: `test_websocket.py collection error: missing python-rapidjson`
- 1 min: `test_db.py failures: missing tzdata package`
- 1 min: `test_dateframe::test_perspective failure: missing anywidget`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
