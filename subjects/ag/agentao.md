# agentao

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/jin-bo/agentao, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/agentao

## Pinned environment

- Project commit: `cd1604bbcf82108a928bca5a243a96e090371a8e`
- Test commit: `cd1604bbcf82108a928bca5a243a96e090371a8e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 5.9 to 5.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2.5 | 5.9 | 3 | 3 | [run](https://argusic.com/run/d4ae14ef-5449-475b-82d1-901d3ae995e1) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `uv not on PATH after pip install to --user`
- 0.5 min: `CLI extra packages (prompt_toolkit, readchar) missing on first agentao invocation`
- 0.5 min: `test_initialize_jieba_redirects_stderr_to_logger failed: ModuleNotFoundError for jieba`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
