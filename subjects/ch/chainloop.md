# chainloop

**Verdict: runs with mocks.** Argusic Score 71 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/chainloop-dev/chainloop, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/chainloop

## Pinned environment

- Project commit: `586d918d3e19185f1d1e9e9ed954fc7f5c9f5cbe`
- Test commit: `586d918d3e19185f1d1e9e9ed954fc7f5c9f5cbe`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 14.8 to 16.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 60 | 7.6 | 14.8 | 1 | 0 | [run](https://argusic.com/run/9e422173-8b9a-48bd-b0cf-a16d0b107de1) |
| 2 | pass with mocks | 82 | 17 | 16.4 | 2 | 1 | [run](https://argusic.com/run/64ce8656-d0f4-43b4-82ee-5aa0f32ce71e) |

## What was observed on a clean machine

Attempt 1:

- `36 test cases fail: rootless Docker not found (testcontainers requires Docker for PostgreSQL, Vault, Minio)`

Attempt 2:

- 1 min: `Go 1.27.1 not installed in container`
- 1 min: `5 test suites fail needing Docker: pkg/blobmanager/s3, pkg/credentials/manager, pkg/credentials/vault, app/controlplane/internal/usercontext, app/artifact-cas/internal/service`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
