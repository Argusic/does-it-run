# wiredoor

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/wiredoor/wiredoor, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/wiredoor

## Pinned environment

- Project commit: `bd01563510987ce85b263bfc71617cb8abdb801c`
- Test commit: `bd01563510987ce85b263bfc71617cb8abdb801c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 8.5 to 8.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 2 | 8.5 | 2 | 2 | [run](https://argusic.com/run/c513f1ff-0f88-4f76-b17c-4a03a83f3097) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `Test setup set PRIVATE_SECRET instead of PRIVATE_KEY env var, causing JWT key generation failure`
- 1 min: `process-manager.ts used raw fs.mkdirSync to /data/oauth2 which fails without root; the mocked FileManager.mkdirSync was not invoked`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
