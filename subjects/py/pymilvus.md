# pymilvus

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/milvus-io/pymilvus, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/pymilvus

## Pinned environment

- Project commit: `9b1d5adeb1ee853d0be00267d002a6fc0909d1e4`
- Test commit: `9b1d5adeb1ee853d0be00267d002a6fc0909d1e4`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 36 to 36 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 34 | 36 | 3 | 3 | [run](https://argusic.com/run/533d1346-7477-46ae-a94a-d500cd52dd88) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `uv not installed; pip refused PEP 668 system install`
- 22 min: `uv sync --group dev initially hung downloading large deps (scipy, pyarrow)`
- 2 min: `make unittest failed: TestGetCommit.test_get_commit AssertionError '290d76f' != 'Get commit for version 2.0.0rc9.dev22 wrong'`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
