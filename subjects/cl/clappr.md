# clappr

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/clappr/clappr, licensed BSD-3-Clause, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/clappr

## Pinned environment

- Project commit: `621ac457d623561976023d3f14045eb7e72da8ad`
- Test commit: `621ac457d623561976023d3f14045eb7e72da8ad`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 7.7 to 7.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 7 | 7.7 | 2 | 2 | [run](https://argusic.com/run/9e39e5be-4d43-4c3b-b3a1-72fcfc914c5f) |

## What was observed on a clean machine

Attempt 1:

- 1.5 min: `Node.js 18.19.1 is installed but project requires >=24 (per .nvmrc)`
- 1.5 min: `@babel/core@8.0.1 engine requires ^22.18.0 || >=24.11.0, v24.0.0 too low`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
