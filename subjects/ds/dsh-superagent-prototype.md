# dsh-superagent-prototype

**Verdict: runs with mocks.** Argusic Score 71 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/deepseek-ai/dsh-superagent-prototype, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/dsh-superagent-prototype

## Pinned environment

- Project commit: `6337fc823ce20251c8de8085948165c81aaa701e`
- Test commit: `6337fc823ce20251c8de8085948165c81aaa701e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 8.6 to 69.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 50 | 8 | 8.6 | 3 | 3 | [run](https://argusic.com/run/4bbad1b4-3613-4503-9115-ccf9a35e01ea) |
| 2 | pass with mocks | 92 | 4.2 | 69.3 | 1 | 1 | [run](https://argusic.com/run/d88bf388-7af1-4456-8ae1-f9faa82b6af1) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node.js v18.19.1 was installed but project requires ^22.19.0 or >=24.0.0; installed Node 22.23.4 via n with N_PREFIX=$HOME/.n`
- 1 min: `pnpm was not installed`
- 3 min: `Feishu event consumer race condition: stderr '[event] ready' arrived after stdout had already processed a malformed JSON line and reported health 'error', overwriting it back to 'ready' , 1 test failed`

Attempt 2:

- 30 min: `tests/sources.spec.ts: feishu malformed-line test fails: expects health.state=="error" when reading a non-JSON event line, but async .catch chain in feishu-loops.ts stdout handler has not settled when the assertion checks health.feishu from`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
