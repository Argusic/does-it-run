# terraform-mcp-server

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/hashicorp/terraform-mcp-server, licensed MPL-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/terraform-mcp-server

## Pinned environment

- Project commit: `d8fd44d71426ccdc8f90d907208a71d2c864f1f6`
- Test commit: `d8fd44d71426ccdc8f90d907208a71d2c864f1f6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 4.4 to 4.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 4.5 | 4.4 | 1 | 1 | [run](https://argusic.com/run/f44c3df7-0e92-4a7a-9b5a-a113b7824560) |

## What was observed on a clean machine

Attempt 1:

- `e2e test suite fails: docker: command not found. The e2e tests require Docker to build a test container image.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
