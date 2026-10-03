# neo

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/neomjs/neo, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/neo

## Pinned environment

- Project commit: `40c1262496c9477a6ff31fb55baafe195fceb4a2`
- Test commit: `40c1262496c9477a6ff31fb55baafe195fceb4a2`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 5.8 to 5.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 5.8 | 2 | 2 | [run](https://argusic.com/run/e58fcbfc-0993-4c20-98a3-a31207407dea) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Container had Node.js v18.19.1 but project requires >=24.0.0`
- `Engine warnings for cssnano/postcss sub-dependencies requiring node ^22.22.3 || ^24.15.0 , Node.js v24.0.0 is borderline`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
