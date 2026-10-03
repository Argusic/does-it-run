# PrismerCloud

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Prismer-AI/PrismerCloud, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/prismercloud

## Pinned environment

- Project commit: `e263666c231c8782fee9e3cc561a1c6a06b384d3`
- Test commit: `e263666c231c8782fee9e3cc561a1c6a06b384d3`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 20.5 to 41.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 41 | 41.1 | 4 | 4 | [run](https://argusic.com/run/c6d490ea-a21a-440d-9dbb-0612503e250e) |
| 2 | pass with mocks | 92 | 20 | 20.5 | 7 | 7 | [run](https://argusic.com/run/c78b8c97-a02e-4c4a-929a-32c44121a678) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `AIP SDK test: crypto.getRandomValues not defined in tsx/Node 18 context`
- 2 min: `AIP SDK build: tsup --dts fails with rollup-plugin-dts on Node 18`
- 5 min: `TS SDK unit tests: 5 realtime tests fail - WebSocket not defined globally`
- 15 min: `Cookbook tests: require PRISMER_API_KEY_TEST env var pointing to prismer.cloud`

Attempt 2:

- 3 min: `WebSocket global not defined in Node 18; TS SDK realtime tests failed`
- 1 min: `opencode-plugin DTS build failed: missing @types/node`
- 2 min: `MCP vitest@5 had incompatible Node version requirement (>=22)`
- 1 min: `Python pip install blocked by externally-managed-environment (Debian)`
- 1 min: `AIP SDK tsup DTS build failed on Node 18 (rollup-plugin-dts incompatibility)`
- 1 min: `Runtime SDK better-sqlite3 native module requires Node >=20`
- `Go and Rust compilers not available in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
