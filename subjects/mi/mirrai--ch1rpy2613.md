# Mirrai

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Ch1rpy2613/Mirrai, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/run/b903a4b9-799e-4ced-9073-1bb8059ade73

## Pinned environment

- Project commit: `03caabe600df1b008cd6139ccd61ff8f12f85306`
- Test commit: `03caabe600df1b008cd6139ccd61ff8f12f85306`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 8 to 8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 12 | 8 | 3 | 3 | [run](https://argusic.com/run/b903a4b9-799e-4ced-9073-1bb8059ade73) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `System Node.js is 18.19.1 but repo requires Node 20+ (vitest.config.ts uses import.meta.dirname, pnpm absent)`
- 4 min: `No PostgreSQL on system and pnpm db:push migration failed against socket path (bad substitution) then socket URL parse broke`
- 3 min: `LLM not configured: chat/analysis would fail with no provider`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
