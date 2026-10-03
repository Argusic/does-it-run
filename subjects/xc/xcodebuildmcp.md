# XcodeBuildMCP

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/getsentry/XcodeBuildMCP, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/xcodebuildmcp

## Pinned environment

- Project commit: `e6ef59b49b44012c824f0a0de261c96142e37390`
- Test commit: `e6ef59b49b44012c824f0a0de261c96142e37390`
- Worker image digests: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`, `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`
- Worker type: cpu
- Test depth: run with mocked services, no run possible
- Valid runs: 3; wall time 14 to 42 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 0.17 | 32.6 | 7 | 7 | [run](https://argusic.com/run/7579f437-0c18-4c3f-95ba-e631e1991dfb) |
| 2 | timeout | none | n/a | 42 | 0 | 0 | [run](https://argusic.com/run/9a9f82f8-4403-4b2e-8afc-d39a8f08bd43) |
| 3 | pass with mocks | 92 | 7.75 | 14 | 5 | 5 | [run](https://argusic.com/run/8b7a3ef9-dbeb-47b4-ab1b-fd6cc2fe9a3b) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `vitest 4.x requires Node 20+ (container has Node 18.19.1)`
- 1 min: `uuid v14 uses crypto.randomUUID() as bare global, not available in vitest worker threads on Node 18`
- 1 min: `yargs-parser 22 requires Node 20+`
- 1 min: `crypto.randomUUID() not available as bare 'crypto' global in vitest forks on Node 18`
- 1 min: `JSON.parse error message differs between Node 18 ('Unexpected token') and newer versions`
- 2 min: `Command runner tests flaky with 250ms timeout under load`
- `ESLint 10 requires Node 20+ (util.styleText not available)`

Attempt 3:

- 2 min: `vitest v4 requires Node 20+ (util.styleText) but container has Node 18.19.1`
- 1 min: `uuid v14 references bare global 'crypto' not available in Node 18 ESM worker threads`
- 1 min: `yargs-parser@22 requires Node 20+ and throws at import on Node 18`
- 1 min: `simulators test expects 'invalid json' but JSON.parse throws 'Unexpected token i in JSON at position 0'`
- 1 min: `ESLint v10 stylish formatter uses util.styleText from Node 20 , breaks on Node 18`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
