# express

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/expressjs/express, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/express

## Pinned environment

- Project commit: `023767fe9872e029271df1418f73401bff20ff40`
- Test commit: `023767fe9872e029271df1418f73401bff20ff40`
- Worker image digests: `sha256:33ceb71981b602c1a7443a53469e4dba065f7503eab3078a2d7a57a2ab987517`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 6; wall time 1 to 12.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.2 | 6.5 | 1 | 1 | [run](https://argusic.com/run/f4517677-af69-4e15-9676-0ff2ed7a32e9) |
| 1 | pass | 100 | 0.23 | 1 | 0 | 0 | [run](https://argusic.com/run/5f0ccee6-f6d6-4bd8-8e7e-d9987d125a90) |
| 2 | pass | 100 | 0.15 | 12.4 | 6 | 6 | [run](https://argusic.com/run/4e43cf30-bc87-4838-8e48-9bc64db2f542) |
| 2 | pass | 100 | 0.13 | 1 | 0 | 0 | [run](https://argusic.com/run/860d1bec-8cd2-48d9-9f94-73ff11e6e4d5) |
| 3 | pass | 100 | 0.2 | 4.6 | 3 | 3 | [run](https://argusic.com/run/82a83c45-fcaa-4e48-ad23-1faeed532c0e) |
| 3 | pass | 100 | 0.14 | 1.4 | 0 | 0 | [run](https://argusic.com/run/c3390442-368b-451a-94b3-015054cec319) |

## What was observed on a clean machine

Attempt 1:

- 6 min: `examples/online crashed with 'TypeError: this.db.multi(...).sadd is not a function' when run per its own documented install ('npm install redis online'); online@0.0.1 expects the pre-v4 node-redis lowercase callback API (multi().sadd/expire`

Attempt 2:

- 6 min: `examples/session/redis.js crashed at require time: 'TypeError: require(...) is not a function' , used the pre-v7 connect-redis factory API while package.json pins connect-redis@^8.0.1, which exports a RedisStore class`
- 5 min: `examples/online/index.js returns 500 on every request: 'TypeError: this.db.multi(...).sadd is not a function' , its own instructions say 'npm install redis online', which today installs redis@6 (promise/camelCase API) while online@0.0.1 dri`
- 2 min: `examples/search and examples/online failed with 'Cannot find module redis' / 'Cannot find module online' , these are optional example-only deps not declared in package.json`
- 8 min: `No Redis available in the container (no redis-server binary, no Docker), blocking examples/search, examples/online and examples/session/redis.js`
- 2 min: `Test-harness self-inflicted: 'pkill -f <pattern>' matched the invoking bash -c command line and killed my own shell (exit 144), twice`
- 3 min: `Test-harness self-inflicted: port-cleanup helper used 'ss', which is not installed in this container, so it silently no-opped and a stale server held port 3000 , one example sweep wrongly reported all 25 examples as EADDRINUSE failures`

Attempt 3:

- 1 min: `EADDRINUSE :::3000 when starting examples/content-negotiation; a previously launched test app still held port 3000 and my pkill -f pattern did not match its cmdline ("node app.js")`
- 2 min: `examples/online failed to boot: Error: Cannot find module 'online' (also requires a running Redis server; no redis-server binary in container)`
- 1 min: `examples/search failed to boot: Error: Cannot find module 'redis' (also requires a running Redis server; no redis-server binary in container)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
