# stashbase

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/liliu-z/stashbase, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/stashbase

## Pinned environment

- Project commit: `21955ea8f4a653c70c673c8fd78bfd2728c243bd`
- Test commit: `21955ea8f4a653c70c673c8fd78bfd2728c243bd`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 11 to 15.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 11 | 0 | 0 | [run](https://argusic.com/run/d33857f7-fcca-4300-a2e1-b48840eec41f) |
| 2 | pass | 100 | 22 | 15.5 | 3 | 3 | [run](https://argusic.com/run/e033c3fb-cd4b-4175-8784-5c754ae92963) |

## What was observed on a clean machine

Attempt 2:

- 3 min: `Node.js v18.19.1 is below required >=24.11.0`
- 2 min: `Python 3.13 not available on system (only 3.12)`
- 1 min: `Electron SUID sandbox helper not configured correctly on Linux container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
