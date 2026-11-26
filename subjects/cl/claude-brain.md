# claude-brain

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/memvid/claude-brain, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/claude-brain

## Pinned environment

- Project commit: `5df71f77aafa4ec50e7fd4672997b6da7e2c3198`
- Test commit: `5df71f77aafa4ec50e7fd4672997b6da7e2c3198`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 5.6 to 8.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2.5 | 8.4 | 1 | 1 | [run](https://argusic.com/run/1928e433-a2e5-4787-8230-829643d696c6) |
| 2 | pass with mocks | 92 | 5 | 5.6 | 5 | 5 | [run](https://argusic.com/run/9d49a07e-2e98-4024-8b95-2043841b1f79) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `smart-install.js hook crashed at runtime: __dirname is not defined in ES module scope`

Attempt 2:

- 1 min: `npm install failed due to zod peer dependency conflict between @memvid/sdk and @langchain/core`
- 1 min: `esbuild install.js postinstall script failed (missing install.js)`
- 1 min: `Lint errors: unnecessary escape characters in session-start.ts`
- 1 min: `ESM __dirname reference error in smart-install.ts`
- 1 min: `TypeScript compilation error in session-start.ts (mangled template literal from prior fix)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
