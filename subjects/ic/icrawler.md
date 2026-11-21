# icrawler

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/hellock/icrawler, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/icrawler

## Pinned environment

- Project commit: `f2a326dc2b0798a5cdb14afd4753af9e86775e66`
- Test commit: `f2a326dc2b0798a5cdb14afd4753af9e86775e66`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 12.4 to 20.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 20.8 | 3 | 3 | [run](https://argusic.com/run/75ba2a21-d833-4466-879f-30961e29f711) |
| 2 | pass | 100 | 0.1 | 12.4 | 3 | 3 | [run](https://argusic.com/run/f0a19f91-61e7-4376-9b05-7f0054430469) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `pip install blocked by externally-managed-environment (Debian PEP 668)`
- 5 min: `Session.request called .format() on None proxy from empty ProxyPool`
- 10 min: `Downloader treated HTTP 200 as error (elif 200 <= response.status_code < 300 caused every successful download to break without saving)`

Attempt 2:

- 3 min: `Session.request() called proxy.format() on None when proxy_pool.get_next() returned None, raising AttributeError`
- 5 min: `Downloader exited on HTTP 200 success without saving the file; break before storage.write()`
- 1 min: `Parser crashed with TypeError iterating over None when parse() returns None instead of a list`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
