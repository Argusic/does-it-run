# TokenHub

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/astaxie/TokenHub, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/tokenhub

## Pinned environment

- Project commit: `08db06008d68b9aa6c5947dbc5069ef451c3a080`
- Test commit: `08db06008d68b9aa6c5947dbc5069ef451c3a080`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 36.5 to 87 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | n/a | 87 | 0 | 0 | [run](https://argusic.com/run/6a1c7fc9-069c-43bf-9a4c-c8226a15b7d6) |
| 2 | pass | 100 | 36.3 | 36.5 | 5 | 5 | [run](https://argusic.com/run/1fd3ab1f-dee4-4b2e-8a5b-de43edb2acb4) |

## What was observed on a clean machine

Attempt 2:

- 3 min: `Go compiler (Go) not found on system`
- 2 min: `Node version too old: v18.19.1, project requires v22.23.1`
- `Frontend component tests (vitest) require Node >=22, failed with Node 18`
- `5 repo gate tool tests fail with Node 18 (TypeScript ESM import not supported)`
- 5 min: `Backend server full test suite times out (>120s) without PostgreSQL - 292 test files contain integration tests requiring external services`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
