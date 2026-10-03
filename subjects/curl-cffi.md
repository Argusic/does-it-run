# curl_cffi

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/lexiforest/curl_cffi, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/curl-cffi

## Pinned environment

- Project commit: `ba87df75970b983e47a80257b89e59e36b0f0d08`
- Test commit: `ba87df75970b983e47a80257b89e59e36b0f0d08`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 38.1 to 38.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 38.1 | 4 | 4 | [run](https://argusic.com/run/bcf43944-77dd-4a5d-a398-e0e4d8cd6bd8) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Source build failed: missing python3.12-dev headers (pyconfig.h) - cannot install system packages without root`
- 3 min: `test_sync_websockets.py failed at collection: WebSocket._MAX_CURL_FRAME_SIZE attribute mismatch between installed wheel and source tree`
- 5 min: `Background /tmp/or-proxy.py process occupied ports needed by test fixtures, causing hangs`
- 10 min: `Several stress/performance tests hang due to resource constraints in container (test_high_parallel, test_high_concurrency, test_huge_payload, test_high_frequency_ping_pong, test_multithreaded_event_loops)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
