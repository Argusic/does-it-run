# react-email-editor

**Verdict: runs.** Argusic Score 94.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/unlayer/react-email-editor, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/react-email-editor

## Pinned environment

- Project commit: `6fa7ae963009a3d7989cd9467f29fb33861541c4`
- Test commit: `6fa7ae963009a3d7989cd9467f29fb33861541c4`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 3; wall time 4 to 4.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 0.6 | 4.2 | 2 | 2 | [run](https://argusic.com/run/b6661dfd-fe9b-4afc-b949-6603ee0f0c9b) |
| 2 | pass with mocks | 92 | 5 | 4.1 | 2 | 2 | [run](https://argusic.com/run/6f7d3105-6699-4bd6-9172-0fd0f322d3e3) |
| 3 | pass | 100 | 3 | 4 | 3 | 3 | [run](https://argusic.com/run/fc47cb80-f4b4-45b4-a30a-1bcfc778c94e) |

## What was observed on a clean machine

Attempt 1:

- 0.1 min: `vitest@4.1.10 incompatible with Node 18.19.1 (uses node:util.styleText added in Node 20)`
- 0.1 min: `jsdom@29.1.1 requires @exodus/bytes (ESM-only) causing ERR_REQUIRE_ESM in CJS context`

Attempt 2:

- 1 min: `vitest@4 requires Node >=20 (container has Node 18.19.1) , rolldown uses node:util.styleText`
- 1 min: `jsdom@29 requires Node >=20 , html-encoding-sniffer uses @exodus/bytes which is ESM-only`

Attempt 3:

- 0.2 min: `Node 18 lacks node:util.styleText needed by vitest 4.x`
- 0.3 min: `Rolldown native binding compiled for Node 18 ABI, fails on Node 22`
- 0.5 min: `jsdom 29 requires --experimental-require-module for ESM-only @exodus/bytes dependency`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
