# deer-flow

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/bytedance/deer-flow, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/deer-flow

## Pinned environment

- Project commit: `3a86278047d230326214e20bd64fceb3156d434e`
- Test commit: `3a86278047d230326214e20bd64fceb3156d434e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 61.7 to 61.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 61.7 | 4 | 4 | [run](https://argusic.com/run/686691bf-5329-43e0-a397-8cc36eef8ee4) |

## What was observed on a clean machine

Attempt 1:

- `Missing prerequisite: nginx not available (no root in container)`
- 1 min: `Pre-installed Node.js 18.19.1 is below the required 22+`
- `Flaky concurrency test: test_concurrent_checkpointer_getter_creates_one_instance times out intermittently`
- `No LLM models configured in config.yaml (fresh copy from template)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
