# authorizer

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/authorizerdev/authorizer, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/authorizer

## Pinned environment

- Project commit: `891f58fdd82b235aafe69bfed2ce085b0a3df25b`
- Test commit: `891f58fdd82b235aafe69bfed2ce085b0a3df25b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 25.4 to 82.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 32 | 82.8 | 0 | 0 | [run](https://argusic.com/run/616de491-3f5c-4402-bd1f-7a45a1574262) |
| 2 | pass | 100 | 18 | 25.4 | 2 | 2 | [run](https://argusic.com/run/104d6075-4c36-448d-b930-8d72c6b85eaa) |

## What was observed on a clean machine

Attempt 2:

- 6 min: `Missing external database containers (PostgreSQL, MongoDB, ArangoDB, ScyllaDB, DynamoDB, Couchbase) for integration tests`
- `MongoDB-specific index tests skipped (connection refused on localhost:27017)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
