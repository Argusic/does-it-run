# unsnooze

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/saaranshM/unsnooze, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/unsnooze

## Pinned environment

- Project commit: `fe3c34f97cf4cb4f86e76734ba44b94b802b4de2`
- Test commit: `fe3c34f97cf4cb4f86e76734ba44b94b802b4de2`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 14 to 14 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 14 | 2 | 2 | [run](https://argusic.com/run/04322aaa-1591-488b-b5c8-7f8ad1948f4d) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Node.js 18.19.1 installed, project requires >=20.12`
- 1 min: `ssh not found on PATH , ssh-detect and fleet tests fail`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
