# exa-mcp-server

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/exa-labs/exa-mcp-server, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/exa-mcp-server

## Pinned environment

- Project commit: `15ffb50519e719dc791cdc750ce5ed1934c0a1ed`
- Test commit: `15ffb50519e719dc791cdc750ce5ed1934c0a1ed`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 3; wall time 2.6 to 7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 4 | 7 | 1 | 1 | [run](https://argusic.com/run/feeb42ed-20a4-455f-9e5d-4dc39f6e4392) |
| 2 | pass with mocks | 92 | 0.5 | 5 | 1 | 1 | [run](https://argusic.com/run/5f47b249-09e3-4eb4-8852-50629cc97469) |
| 3 | pass with mocks | 92 | 0.12 | 2.6 | 1 | 1 | [run](https://argusic.com/run/b2d078b0-36a7-4fbd-8f38-c6081b5f3225) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `4 test failures in errorHandler.test.ts due to afterEach hook timeout with vi.useFakeTimers`

Attempt 2:

- 0.1 min: `4 vitest tests hung on afterEach(vi.useRealTimers) hook , vitest 4.x incompatibility`

Attempt 3:

- 2 min: `tests/unit/utils/errorHandler.test.ts: afterEach hook timed out , vi.useFakeTimers() in test bodies conflicted with vitest 4.x internal timer usage`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
