# dashi-taskboard

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/chuspeeism/dashi-taskboard, licensed Apache-2.0, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/dashi-taskboard

## Pinned environment

- Project commit: `723c400eec86c454c1ffa56ee1b500746d41e142`
- Test commit: `723c400eec86c454c1ffa56ee1b500746d41e142`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 3.3 to 6.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 45 | 6.1 | 3 | 3 | [run](https://argusic.com/run/3306c0a8-bbd3-4176-8f9f-290716d8e8f9) |
| 2 | pass | 100 | 5 | 3.3 | 1 | 1 | [run](https://argusic.com/run/5e27aadd-47e8-4d6f-b5fd-f3fc63ae50a6) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `System Node.js 18.19.1 does not meet >=22.5 requirement`
- 2 min: `Rollup native binding @rolldown/binding-linux-x64-gnu not installed as optional dependency`
- 2 min: `node:sqlite built-in requires --experimental-sqlite flag`

Attempt 2:

- 1 min: `System Node.js v18 does not meet project requirement of >=22.5`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
