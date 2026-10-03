# codex-chatgpt-web

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/miuuyy/codex-chatgpt-web, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/codex-chatgpt-web

## Pinned environment

- Project commit: `a13cd09950969f43e3b7e25c71fa43efaf5446c5`
- Test commit: `a13cd09950969f43e3b7e25c71fa43efaf5446c5`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 7.5 to 7.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 1.5 | 7.5 | 2 | 2 | [run](https://argusic.com/run/d8af7afe-e1d7-48a7-b8cc-69692248efbd) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Bun not installed in container - requires unzip which needs root`
- 0.5 min: `package.json pinned bun@1.4.0 but installed bun@1.4.2; verify script rejected mismatched versions`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
