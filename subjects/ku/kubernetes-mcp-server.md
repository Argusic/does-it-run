# kubernetes-mcp-server

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/containers/kubernetes-mcp-server, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/kubernetes-mcp-server

## Pinned environment

- Project commit: `f4a39b17ca4cb60e1bfa83bd2eabd725a352d22d`
- Test commit: `f4a39b17ca4cb60e1bfa83bd2eabd725a352d22d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 15.1 to 29.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 28 | 29.2 | 3 | 3 | [run](https://argusic.com/run/9128d870-b930-4445-859d-abee6fd04c0e) |
| 2 | pass with mocks | 92 | 20 | 15.1 | 2 | 2 | [run](https://argusic.com/run/f387a15f-fbf6-4616-a007-0bb5c5b494f4) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `No Go compiler found in container`
- 2 min: `make build failed at lint step: 'parallel golangci-lint is running' due to stale process from earlier run`
- 5 min: `3 test suites failing: pkg/http, pkg/kubernetes-mcp-server/cmd (TestHTTPSIGHUP) - all failed with 'dial tcp [::]:port: connect: cannot assign requested address' because IPv6 is disabled in container but test helpers defaulted to IPv6`

Attempt 2:

- 3 min: `Go binary not found in container PATH`
- 2 min: `IPv6 disabled in container causes net.DialTCP('tcp',...) to fail with 'cannot assign requested address' in HTTP tests`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
