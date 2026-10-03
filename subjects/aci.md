# aci

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/aipotheosis-labs/aci, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/aci

## Pinned environment

- Project commit: `3e4a82fa5fd22f1165af2b39fa3de2b0f031242e`
- Test commit: `3e4a82fa5fd22f1165af2b39fa3de2b0f031242e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 37.2 to 37.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 8 | 37.2 | 6 | 6 | [run](https://argusic.com/run/de9b7d61-248b-48b4-a990-3b619e3cdcfe) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `PostgreSQL+pgvector not pre-installed`
- 5 min: `test-db hostname not resolvable without Docker`
- 5 min: `Propelauth mock server required for auth`
- 5 min: `AWS KMS not available without Docker/LocalStack`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
