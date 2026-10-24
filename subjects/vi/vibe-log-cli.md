# vibe-log-cli

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/vibe-log/vibe-log-cli, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/vibe-log-cli

## Pinned environment

- Project commit: `0354df12d7747d24023d71a996f6e6a011500843`
- Test commit: `0354df12d7747d24023d71a996f6e6a011500843`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 23.5 to 23.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 1 | 23.5 | 3 | 3 | [run](https://argusic.com/run/7d01ced7-e90e-4924-83c3-68610f9a9405) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `vitest 3.x requires Node 20+ (container has Node 18.19.1)`
- 10 min: `3 test files with 8 test failures due to mock lifecycle and module reload issues`
- 5 min: `@agentclientprotocol/sdk is ESM-only but tsup emitted CJS, causing ERR_REQUIRE_ESM at runtime`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
