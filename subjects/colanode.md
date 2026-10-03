# colanode

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/colanode/colanode, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/colanode

## Pinned environment

- Project commit: `d649523637f0f059c936418488165d4a689da27c`
- Test commit: `d649523637f0f059c936418488165d4a689da27c`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 3; wall time 10 to 30.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 28 | 30.4 | 3 | 3 | [run](https://argusic.com/run/4d45114a-a6cd-4dc1-99b6-5d23883ae1cb) |
| 2 | pass | 100 | 3 | 10 | 3 | 3 | [run](https://argusic.com/run/ec17650c-7694-4f2c-9a14-ba574b5d1db7) |
| 3 | pass | 100 | 4.1 | 14.9 | 2 | 2 | [run](https://argusic.com/run/52e6e0ce-8b69-4d1b-9e82-fa2db068d3a0) |

## What was observed on a clean machine

Attempt 1:

- 12 min: `better-sqlite3 native module compilation failed: missing build tools (make, gcc, g++) and no apt-get/sudo available. This package is only required by 'scripts' and 'apps/desktop' workspaces, not by server or web.`
- 8 min: `jsdom@28.1.0 uses html-encoding-sniffer@6 which require()-loads an ESM-only @exodus/bytes/encoding-lite.js , Node 18 cannot CJS-require an ESM module.`
- 5 min: `Server tests require Docker (Testcontainers for Postgres+Redis) which is unavailable in this container. Also undici@7 (used by testcontainers) requires Node >= 20 for the File global.`

Attempt 2:

- 1 min: `Node.js v18.19.1 incompatible with engine requirements (needs ^20.19.0 || ^22.12.0 || >=24.0.0)`
- `Docker not available: server tests require Testcontainers for Postgres+Redis containers, and server runtime requires Postgres+Redis`
- `Desktop app launch blocked: Electron sandbox not configured and dbus not available`

Attempt 3:

- 4.1 min: `Node 18 incompatible with @asamuzakjp/css-color requiring >=20.19.0`
- 0.8 min: `Package outputs not built; TS6305 errors on compile`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
