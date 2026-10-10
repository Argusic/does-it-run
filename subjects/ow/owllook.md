# owllook

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/howie6879/owllook, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/owllook

## Pinned environment

- Project commit: `ef8eea67a5071500aec146d5ac8ec4213c77f6b0`
- Test commit: `ef8eea67a5071500aec146d5ac8ec4213c77f6b0`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 15 to 15 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 14.7 | 15 | 7 | 7 | [run](https://argusic.com/run/e81a175a-e946-46a0-8956-658174061653) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `config/__init__.py forced MODE='PRO' and fell back to base Config class missing REDIS_DICT/MONGODB`
- 8 min: `aioredis 0.3.3 and asyncio_redis 0.14.3 use asyncio.async (reserved keyword) and asyncio.coroutine (removed in Python 3.12)`
- 3 min: `sanic 0.5.1 HttpProtocol __slots__ missing error_handler, _last_request_time, _request_handler_task`
- 5 min: `aioredis/pool.py Lock() and Event() accept loop=loop kwarg removed in Python 3.12`
- 1 min: `Jinja2 2.11.3 PackageLoader requires pkg_resources from setuptools`
- 3 min: `aioredis 0.3 pool uses yield-from-based Python 2-style coroutines incompatible with Python 3.12`
- 1 min: `Test used asyncio.get_event_loop() which fails in Python 3.12`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
