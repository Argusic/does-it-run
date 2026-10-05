# minimax-code

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/MiniMax-AI/minimax-code, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/minimax-code

## Pinned environment

- Project commit: `0f6ad5229ff1f144c72dd15a4b2d520feb26cd3d`
- Test commit: `0f6ad5229ff1f144c72dd15a4b2d520feb26cd3d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 27.3 to 27.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2.5 | 27.3 | 2 | 2 | [run](https://argusic.com/run/e0efb1ac-df75-4cdf-9f9e-942410bd1c85) |

## What was observed on a clean machine

Attempt 1:

- 2.5 min: `Node.js 18.19.1 is too old (requires >=22.19). Installed nvm and Node.js 22.19.0.`
- `Pre-existing test failure: 'caps a large nonzero-exit result' in packages/agent-tools/test/desktop/local-bash-output.test.ts , the head/tail truncation budget at 24KB max (22KB preview) cannot fit expectation 'error-row-399-' alongside 'err`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
