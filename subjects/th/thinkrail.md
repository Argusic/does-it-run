# thinkrail

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/JetBrains/thinkrail, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/thinkrail

## Pinned environment

- Project commit: `cd73167a085ec6a7d13799e215fe0fac25cde695`
- Test commit: `cd73167a085ec6a7d13799e215fe0fac25cde695`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 17.7 to 17.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 17.9 | 0 | 0 | [run](https://argusic.com/run/03f79cb3-e366-4ae1-a42e-4259416ec981) |
| 2 | pass | 100 | 17 | 17.7 | 2 | 2 | [run](https://argusic.com/run/486d1b8b-d006-4fe9-809d-63828aefdbcc) |

## What was observed on a clean machine

Attempt 2:

- 5 min: `Node.js v18.19.1 below pi requirement (22.19+) and vite requirement (20.19+). Vite build via turbo fails with ReferenceError: CustomEvent`
- 1 min: `unzip missing - bun install via curl failed`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
