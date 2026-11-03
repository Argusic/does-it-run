# codex-chatgpt-web

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/miuuyy/codex-chatgpt-web, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/codex-chatgpt-web

## Pinned environment

- Project commit: `a13cd09950969f43e3b7e25c71fa43efaf5446c5`
- Test commit: `a13cd09950969f43e3b7e25c71fa43efaf5446c5`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 7.5 to 9.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 1.5 | 7.5 | 2 | 2 | [run](https://argusic.com/run/d8af7afe-e1d7-48a7-b8cc-69692248efbd) |
| 2 | pass | 100 | 3.2 | 9.2 | 3 | 3 | [run](https://argusic.com/run/67dde98d-5f5a-4152-b6a7-9f86d566f0b3) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Bun not installed in container - requires unzip which needs root`
- 0.5 min: `package.json pinned bun@1.4.0 but installed bun@1.4.2; verify script rejected mismatched versions`

Attempt 2:

- 1.5 min: `Bun 1.4.4 installed initially but project requires 1.4.0`
- 0.8 min: `Node 18 can't resolve @electron/get ESM module during electron postinstall`
- `7 launcher tests fail due to incomplete Electron mock (powerSaveBlocker.isStarted not a function, etc.)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
