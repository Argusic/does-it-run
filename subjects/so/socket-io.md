# socket.io

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/socketio/socket.io, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/socket-io

## Pinned environment

- Project commit: `1eaa582d3b453e3e6f522300ed05b10da0a0799b`
- Test commit: `1eaa582d3b453e3e6f522300ed05b10da0a0799b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 30 to 30 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 29.1 | 30 | 9 | 9 | [run](https://argusic.com/run/75349f8b-d94b-46b0-8cf1-6221689208e4) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `npm ci failed: package-lock.json out of sync with package.json; missing puppeteer-core and chromium-bidi packages`
- 1 min: `npm install (with scripts) failed: @fails-components/webtransport-transport-http3-quiche build.js uses 'import with' syntax unsupported by Node 18`
- 1.5 min: `engine.io WebTransport tests fail: native QUIC module (webtransport.node) cannot be built on Node 18`
- 0.5 min: `engine.io-client WebTransport tests fail: same native module issue`
- 3 min: `engine.io-client test hooks failed: serialize-javascript@7.x uses bare 'crypto' global undefined in strict mode on Node 18`
- 1.5 min: `socket.io tests fail: uWebSockets.js native binary incompatible with Node 18`
- `@socket.io/cluster-engine redis tests fail: no Redis server available`
- `@socket.io/postgres-emitter tests fail: needs PostgreSQL server`
- `@socket.io/redis-streams-emitter no tests discovered: requires Redis server`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
