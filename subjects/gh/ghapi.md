# ghapi

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/AnswerDotAI/ghapi, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/ghapi

## Pinned environment

- Project commit: `81b28a5325b311e9878a676a57fef801093242f6`
- Test commit: `81b28a5325b311e9878a676a57fef801093242f6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 3.5 to 6.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 6 | 6.6 | 4 | 4 | [run](https://argusic.com/run/b7e342dc-11ba-4ba5-8096-8c6773bca894) |
| 2 | pass | 100 | 0 | 3.5 | 3 | 3 | [run](https://argusic.com/run/d58f5203-6e44-4571-82f9-1e23951368bd) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `System pip refused install due to externally-managed-environment (PEP 668)`
- 1 min: `fastgit not installed initially, needed by skill module`
- 1 min: `pyskills not installed initially, needed by skill module`
- 1 min: `pytest not available for test execution`

Attempt 2:

- `Could not import GhAuth from ghapi.auth (no such class)`
- `GhApi(sync=True) has no 'sync' attribute`
- `GraphQL module requires GITHUB_TOKEN`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
