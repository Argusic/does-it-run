# tianji

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/msgbyte/tianji, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/tianji

## Pinned environment

- Project commit: `1aba241d9a79d9c0e2c95f0721fbb4cef31e98a3`
- Test commit: `1aba241d9a79d9c0e2c95f0721fbb4cef31e98a3`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 24.8 to 34.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 35 | 34.7 | 6 | 6 | [run](https://argusic.com/run/08f05761-4a9f-4eb1-a732-096735c6cdce) |
| 2 | pass with mocks | 92 | 15 | 24.8 | 3 | 3 | [run](https://argusic.com/run/566618a8-5db9-454c-9e40-f0dab3324b2b) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Node.js v18 installed but project requires Node 22.14+`
- 1 min: `pnpm test command failed because vitest binary not resolved from root`
- 1 min: `server type check caused OOM`
- 1 min: `client build caused OOM`
- 10 min: `PostgreSQL required for database-dependent tests`
- 1 min: `4 snapshot mismatches in warehouse insight SQL builder tests due to current-date offset`

Attempt 2:

- 2 min: `isolated-vm native build failed: missing -lz, -lbrotlidec, -lbrotlienc, -lcares, -lnghttp2, -licui18n, -licuuc, -licudata`
- 2 min: `Node.js v18.19.1 too old (requires >=22.14.0)`
- `Server segfaults on start without PostgreSQL (DATABASE_URL not set)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
