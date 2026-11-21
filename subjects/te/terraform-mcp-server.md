# terraform-mcp-server

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/hashicorp/terraform-mcp-server, licensed MPL-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/terraform-mcp-server

## Pinned environment

- Project commit: `d8fd44d71426ccdc8f90d907208a71d2c864f1f6`
- Test commit: `d8fd44d71426ccdc8f90d907208a71d2c864f1f6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 4.4 to 10.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 4.5 | 4.4 | 1 | 1 | [run](https://argusic.com/run/f44c3df7-0e92-4a7a-9b5a-a113b7824560) |
| 2 | pass | 100 | 9 | 10.1 | 2 | 2 | [run](https://argusic.com/run/9048b730-d8ce-4a97-81c8-ec3cecba77c6) |

## What was observed on a clean machine

Attempt 1:

- `e2e test suite fails: docker: command not found. The e2e tests require Docker to build a test container image.`

Attempt 2:

- 2 min: `Go 1.26.6 not installed in container`
- `e2e tests require Docker (not available in container)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
