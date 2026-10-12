# sdk-go

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/temporalio/sdk-go, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/sdk-go

## Pinned environment

- Project commit: `626130f1fd9de50cfd90b884a3fb796504f22dc1`
- Test commit: `626130f1fd9de50cfd90b884a3fb796504f22dc1`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 29.1 to 29.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8 | 29.1 | 3 | 3 | [run](https://argusic.com/run/5785534b-2a41-426d-b90b-d592258a5828) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `go toolchain not found (go.mod requires go 1.26.0)`
- 1 min: `assumed build tool is runnable from repo root; repo canonical usage is from internal/cmd/build`
- 2 min: `attempted -run TestIntegrationSuite/TestStartWorkflow which matched no tests (“no tests to run”), not counted as verification`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
