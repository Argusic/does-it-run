# pipecd

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/pipe-cd/pipecd, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/pipecd

## Pinned environment

- Project commit: `c007af06630d0a87baec02db812ed7430db6dbde`
- Test commit: `c007af06630d0a87baec02db812ed7430db6dbde`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 49.6 to 49.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 37 | 49.6 | 6 | 6 | [run](https://argusic.com/run/79af11af-1038-494d-b4ca-aac8e79a7b89) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `go toolchain not installed in container`
- 9 min: `unzip missing: terraform toolregistry test failed ("/bin/sh: 4: unzip: not found")`
- 8 min: `envtest/etcd missing: TestExecutor_ensureSync failed (fork/exec /usr/local/kubebuilder/bin/etcd: no such file or directory)`
- 8 min: `Node v18 too old for web app (requires >=24.10.0), yarn missing`
- 4 min: `yarn --cwd web build fails when running from repo root (package.json contains PIPECD_VERSION= backticks executed in cwd: 'git rev-parse --short HEAD' returned fatal error)`
- 7 min: `pkg/oci test requires Docker daemon (dial unix /var/run/docker.sock: no such file or directory); rootlesskit blocked (Operation not permitted)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
