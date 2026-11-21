# MyTube

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/franklioxygen/MyTube, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/mytube

## Pinned environment

- Project commit: `cd7b43594f1f2d0c92ef2f7acd329d8a1797f625`
- Test commit: `cd7b43594f1f2d0c92ef2f7acd329d8a1797f625`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 6.4 to 44.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 22 | 44.3 | 0 | 0 | [run](https://argusic.com/run/273ea021-983e-4c9a-b5b2-8b454f298db7) |
| 2 | pass | 100 | 6 | 6.4 | 2 | 2 | [run](https://argusic.com/run/74f99d28-7ef7-4e42-9663-8cc38e0ecb63) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `Node.js v18.19.1 in container too old (project requires >=22.22.0)`
- `backend/.env had placeholder PORT={backend_port}`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
