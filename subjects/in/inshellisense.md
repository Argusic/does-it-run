# inshellisense

**Verdict: runs.** Argusic Score 90 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/microsoft/inshellisense, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/inshellisense

## Pinned environment

- Project commit: `63872c52ebc83389735998ade5486f1bd069d0bf`
- Test commit: `63872c52ebc83389735998ade5486f1bd069d0bf`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 5.2 to 5.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 90 | 8 | 5.2 | 2 | 1 | [run](https://argusic.com/run/34d8b0e0-f4bd-4678-8088-4c9def748d87) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `node:sea static import fails on Node 18`
- 2 min: `@microsoft/tui-test requires Node >=20 for native binary`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
