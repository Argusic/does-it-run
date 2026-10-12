# ClawBench

**Verdict: runs with mocks.** Argusic Score 72 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/TIGER-AI-Lab/ClawBench, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/clawbench

## Pinned environment

- Project commit: `187cd252bc60af8ac3a2c98a87c9316e49a5ac75`
- Test commit: `187cd252bc60af8ac3a2c98a87c9316e49a5ac75`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 2.6 to 2.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 72 | 7 | 2.6 | 1 | 0 | [run](https://argusic.com/run/1f237645-aba3-4d16-9538-b7bfb94ef378) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `One test (test_batch_stays_importable_without_a_container_engine) shows non-deterministic ordering sensitivity , fails when run in isolation after other host_timeout tests but passes in full suite run. Not a code defect, test isolation edge`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
