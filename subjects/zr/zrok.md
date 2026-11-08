# zrok

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/openziti/zrok, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/zrok

## Pinned environment

- Project commit: `3bd9152ea9465ce0e46c529b0fd9e9bd00e40a7e`
- Test commit: `3bd9152ea9465ce0e46c529b0fd9e9bd00e40a7e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 11.3 to 27.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 10 | 11.3 | 0 | 0 | [run](https://argusic.com/run/bbd1efd2-6118-4bb5-850c-4db95b6fda2c) |
| 2 | pass with mocks | 92 | 42 | 27.2 | 5 | 5 | [run](https://argusic.com/run/bc2895dc-1280-4380-b410-d2e57d3f164a) |

## What was observed on a clean machine

Attempt 2:

- 5 min: `go not installed in container`
- 8 min: `controller TLS failed: zrok controller rejected mock edge cert x509: certificate signed by unknown authority`
- 12 min: `zrok2 enable failed with 500 error creating environment identity status 200 (mock lacked POST /identities), then token signature is invalid (JWT signed with wrong key), then expected 1 or more CAs from controller, got 0 (missing client well`
- 8 min: `zrok2 share public 500 CHECK constraint failed chk_z_id (mock returned no service/policy IDs)`
- 9 min: `zrok2 share proxy failed at client overlay dial: no apiSession, authentication attempt failed status 404 because the OpenZiti edge/fabric itself cannot run in this container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
