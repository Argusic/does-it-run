# kener

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/rajnandan1/kener, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/kener

## Pinned environment

- Project commit: `eec52e6a70729c5b639feb20aeccaf3a25ccf76e`
- Test commit: `eec52e6a70729c5b639feb20aeccaf3a25ccf76e`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 3; wall time 13.5 to 38.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 20.5 | 24.2 | 5 | 5 | [run](https://argusic.com/run/b8f5d798-4ebb-427a-ab1f-a84925ef43ff) |
| 2 | pass | 100 | 35 | 38.9 | 3 | 3 | [run](https://argusic.com/run/2d4f8aac-bd67-40d9-a1e4-adf67aa7df21) |
| 3 | pass | 100 | 12 | 13.5 | 5 | 5 | [run](https://argusic.com/run/974598cd-4af6-4e2f-b8d6-134de3c49978) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Node.js version 18.19.1 did not meet required >=20`
- 1 min: `svelte-awesome-color-picker required Node >=24`
- 2 min: `npm install scripts not auto-approved for bcrypt, better-sqlite3, esbuild, sharp`
- 3 min: `Redis server not installed in container`
- 5 min: `Client (browser) tests fail: libglib-2.0.so.0 missing for Chromium headless shell`

Attempt 2:

- 2 min: `System Node.js v18 incompatible (project requires >=20, dependency svelte-awesome-color-picker requires >=24)`
- 8 min: `BullMQ background schedulers crashed process on startup due to unhandled rejections and Lua script errors`
- 12 min: `Redis required by BullMQ queues but unavailable; mock RESP servers had parsing bugs with BullMQ's EVALSHA protocol`

Attempt 3:

- 2 min: `Node.js v18.19.1 too old (requires >=20)`
- 1 min: `better-sqlite3 segfault after Node upgrade (stale native binary)`
- 2 min: `Migration .ts files not loadable by production Node ESM loader`
- 5 min: `No Redis server available`
- `Seed .ts files not loadable in production (vite-node not in bundle)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
