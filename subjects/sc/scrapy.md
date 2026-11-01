# scrapy

**Verdict: runs.** Argusic Score 90 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/scrapy/scrapy, licensed BSD-3-Clause, written in Python.

Evidence and recordings: https://argusic.com/subject/scrapy

## Pinned environment

- Project commit: `08f0636b821cb1bc829c593e0382653e4058ab6f`
- Test commit: `08f0636b821cb1bc829c593e0382653e4058ab6f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 11.2 to 14.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 80 | 1 | 11.2 | 1 | 0 | [run](https://argusic.com/run/a175bb1d-cee0-4268-abff-6d57c3cc15f2) |
| 2 | pass | 100 | 3 | 14.6 | 2 | 2 | [run](https://argusic.com/run/961125a3-af48-4c4d-8cd6-a8dd390b4c39) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `test_download_conn_failed fails because container has IPv6 disabled; Twisted gets EADDRNOTAVAIL (errno 99) instead of ECONNREFUSED`

Attempt 2:

- 1 min: `pytest 9.2.0 incompatible with Scrapy test fixtures (session-scoped fixture instance methods deprecated) causing 37 test errors`
- `test_download_conn_failed fails with ConnectError (Errno 99 Cannot assign requested address) in container - IPv6 localhost connect returns wrong errno`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
