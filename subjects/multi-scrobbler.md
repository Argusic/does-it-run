# multi-scrobbler

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/FoxxMD/multi-scrobbler, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/multi-scrobbler

## Pinned environment

- Project commit: `8d7b911a3aa4d2bcfa35a212a536cd5ac2816bbd`
- Test commit: `8d7b911a3aa4d2bcfa35a212a536cd5ac2816bbd`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 4.2 to 8.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1 | 4.2 | 1 | 1 | [run](https://argusic.com/run/e712b067-ee70-4361-b14a-15e294e54b5d) |
| 2 | pass | 100 | 2.5 | 8.8 | 1 | 1 | [run](https://argusic.com/run/8570103e-8540-4b23-8651-0500dca2fed6) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Container had Node.js v18.19.1 but project requires >=24.14.0`

Attempt 2:

- 1.5 min: `System Node.js (v18.19.1) below minimum v24.14.0 required by package.json`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
