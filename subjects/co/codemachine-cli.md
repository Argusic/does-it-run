# CodeMachine-CLI

**Verdict: could not verify.** Argusic Score 75 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/moazbuilds/CodeMachine-CLI, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/codemachine-cli

## Pinned environment

- Project commit: `572def63eb808e95b18ccf6c69a13d7a13fe06fd`
- Test commit: `572def63eb808e95b18ccf6c69a13d7a13fe06fd`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 2; wall time 3.7 to 4.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 70 | 5 | 3.7 | 2 | 1 | [run](https://argusic.com/run/cd949ee4-6a59-40f2-9fdc-3124d8abc317) |
| 2 | fail | 80 | 3 | 4.8 | 0 | 0 | [run](https://argusic.com/run/c001f0fc-895a-4c2f-bc08-a6819c56922e) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Bun runtime not pre-installed`
- `10 TypeScript compilation errors (tsc --noEmit)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
