# ruia

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/howie6879/ruia, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/ruia

## Pinned environment

- Project commit: `68a45028830a6e6b88eda00abf021174a8ceaceb`
- Test commit: `68a45028830a6e6b88eda00abf021174a8ceaceb`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 22 to 22 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 37 | 22 | 7 | 7 | [run](https://argusic.com/run/497caf06-acdd-484e-9689-fa826c3308ee) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `pip install failed: externally-managed-environment (PEP 668)`
- 1 min: `Missing dependency: async-timeout not listed in setup.py install_requires`
- 5 min: `All network tests crashed: asyncio.get_event_loop() raised RuntimeError on Python 3.12 + uvloop`
- 2 min: `Spider.__init__ creates ClientSession() without loop arg; aiohttp 3.14 requires running loop or explicit loop param`
- 3 min: `start_worker() in spider.py had AttributeError: 'Response' object has no attribute 'close_request' when handle_callback results (2-tuples) were mixed with handle_request results (3-tuples)`
- 2 min: `test_response.py had module-level get_event_loop() calls that fail during pytest collection`
- `test_request_url fails: HN changed HTML from a.storylink to span.titleline a`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
