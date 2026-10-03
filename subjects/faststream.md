# faststream

**Verdict: runs.** Argusic Score 80 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ag2ai/faststream, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/faststream

## Pinned environment

- Project commit: `31df8dac071bb47d05537afdf8fa50b36eda6354`
- Test commit: `31df8dac071bb47d05537afdf8fa50b36eda6354`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 41.9 to 41.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 80 | 0.22 | 41.9 | 1 | 0 | [run](https://argusic.com/run/6ae9f1ff-87f9-4110-86bf-1a3a4fd03f1f) |

## What was observed on a clean machine

Attempt 1:

- `test_serve_asyncapi_docs_from_app_with_reload fails on first run due to missing @pytest.mark.slow() marker and --reload file-watcher startup timing`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
