# deer-workflow

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/deerwork-ai/deer-workflow, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/deer-workflow

## Pinned environment

- Project commit: `b20823012eeec15d41f4969f09964401e00f56e0`
- Test commit: `b20823012eeec15d41f4969f09964401e00f56e0`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 1.7 to 4.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1.5 | 1.7 | 0 | 0 | [run](https://argusic.com/run/53317134-6549-43e8-9b6f-67d2fd4b0762) |
| 2 | pass with mocks | 92 | 1 | 4.3 | 1 | 1 | [run](https://argusic.com/run/ef642e2e-32f7-429a-b309-7fb0f533e08e) |

## What was observed on a clean machine

Attempt 2:

- 0.5 min: `bunx symlink was not created by manual Bun install (zip extraction)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
