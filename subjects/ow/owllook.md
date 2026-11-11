# owllook

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/howie6879/owllook, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/owllook

## Pinned environment

- Project commit: `ef8eea67a5071500aec146d5ac8ec4213c77f6b0`
- Test commit: `ef8eea67a5071500aec146d5ac8ec4213c77f6b0`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 13.8 to 15 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 14.7 | 15 | 7 | 7 | [run](https://argusic.com/run/e81a175a-e946-46a0-8956-658174061653) |
| 2 | pass with mocks | 92 | 6 | 13.8 | 12 | 12 | [run](https://argusic.com/run/b37bcb81-8093-4104-b439-b6627af02ca1) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `config/__init__.py forced MODE='PRO' and fell back to base Config class missing REDIS_DICT/MONGODB`
- 8 min: `aioredis 0.3.3 and asyncio_redis 0.14.3 use asyncio.async (reserved keyword) and asyncio.coroutine (removed in Python 3.12)`
- 3 min: `sanic 0.5.1 HttpProtocol __slots__ missing error_handler, _last_request_time, _request_handler_task`
- 5 min: `aioredis/pool.py Lock() and Event() accept loop=loop kwarg removed in Python 3.12`
- 1 min: `Jinja2 2.11.3 PackageLoader requires pkg_resources from setuptools`
- 3 min: `aioredis 0.3 pool uses yield-from-based Python 2-style coroutines incompatible with Python 3.12`
- 1 min: `Test used asyncio.get_event_loop() which fails in Python 3.12`

Attempt 2:

- 1 min: `Pipfile pointed at pypi.douban.com which was unreachable`
- 1 min: `Missing pro_config.py needed by PRO mode`
- 0.5 min: `Python 3.12 removed asyncio.get_event_loop() for new event loops`
- 2 min: `aioredis 0.3.x uses 'asyncio.async' removed in 3.12`
- 1.5 min: `aiocache 0.3.2 used 'aiocache.log.logger' and 'aiocache.utils', removed in 0.12.x`
- 1.5 min: `sanic 0.5.1 depended on old websockets API ('handshake' module)`
- 1 min: `sanic_session 0.4.1 requires aioredis at import time`
- 0.5 min: `sanic 23+ Request objects lack __getitem__/__setitem__`
- 1 min: `Jinja2 2.11.3 uses PackageLoader which broke with its API`
- 0.5 min: `async_timeout 5.x requires 'async with' not 'with'`
- 5 min: `No MongoDB or Redis services available in container`
- 0.5 min: `aiocache cached decorator key building failed when key_from_attr was set but function had no args`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
