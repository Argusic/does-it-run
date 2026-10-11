# langsmith-sdk

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/langchain-ai/langsmith-sdk, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/langsmith-sdk

## Pinned environment

- Project commit: `c51e722026138478b728884d9a3b504ef2ba8ea0`
- Test commit: `c51e722026138478b728884d9a3b504ef2ba8ea0`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 44.9 to 44.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 40 | 44.9 | 5 | 5 | [run](https://argusic.com/run/486fbb50-1cd6-45fe-a484-1e710835203f) |

## What was observed on a clean machine

Attempt 1:

- 10 min: `pytest_httpx cannot mock httpx2 transport (RetryTransport creates inner HTTPTransport at __init__ time)`
- 5 min: `JS Jest tests fail: crypto.randomUUID undefined in Node 18`
- 1 min: `test_strands_agents cannot import: no 'strands' module installed`
- 2 min: `test_google_adk cannot import: no 'google.adk' module`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
