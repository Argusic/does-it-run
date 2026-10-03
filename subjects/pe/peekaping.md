# peekaping

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/0xfurai/peekaping, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/peekaping

## Pinned environment

- Project commit: `742a60d94fdaacc977c09444b651f7cf1c1aab9e`
- Test commit: `742a60d94fdaacc977c09444b651f7cf1c1aab9e`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 15.7 to 17.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 15 | 17.5 | 0 | 0 | [run](https://argusic.com/run/d531e1d1-f868-4976-b501-92743e350f76) |
| 2 | pass | 100 | 22 | 15.7 | 6 | 6 | [run](https://argusic.com/run/29b32613-4c7f-41a8-9c03-5067133e16fe) |

## What was observed on a clean machine

Attempt 2:

- 5 min: `Go compiler not installed`
- 2 min: `Node.js v18.19.1 is below required v20.18.0`
- 1 min: `pnpm not found`
- 6 min: `Redis not available`
- 1 min: `Config validation failed: missing DB_TYPE, DB_NAME`
- 2 min: `Database tables missing (starting server failed on 'no such table: settings')`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
