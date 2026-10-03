# proxy.py

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/abhinavsingh/proxy.py, licensed BSD-3-Clause, written in Python.

Evidence and recordings: https://argusic.com/subject/proxy-py

## Pinned environment

- Project commit: `fec682bc7d702a934eafcf8ad6f1fba835ebef91`
- Test commit: `fec682bc7d702a934eafcf8ad6f1fba835ebef91`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 9.1 to 9.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.5 | 9.1 | 1 | 1 | [run](https://argusic.com/run/3b47ab95-c18a-40f5-84fc-69c403248156) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `test_wait_for_server_raises_timeout_error failed with OSError: [Errno 99] Cannot assign requested address`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
