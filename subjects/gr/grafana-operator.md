# grafana-operator

**Verdict: runs.** Argusic Score 92.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/grafana/grafana-operator, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/grafana-operator

## Pinned environment

- Project commit: `5c12c7397bc9c470e3dda705a71efcbd6cb033fb`
- Test commit: `5c12c7397bc9c470e3dda705a71efcbd6cb033fb`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 5.3 to 12.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 85.33 | 12 | 12.9 | 3 | 2 | [run](https://argusic.com/run/40709473-5e33-46ca-a8e5-0927243919b0) |
| 2 | pass | 100 | 5 | 5.3 | 0 | 0 | [run](https://argusic.com/run/fdecf5f3-a580-408d-a095-c69d65122572) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Go 1.27.1 binary not found on system`
- 2 min: `kubebuilder test binaries (etcd, kube-apiserver, kubectl) not found at /usr/local/kubebuilder/bin`
- `Docker not available: controller integration tests (TestContainers) require Docker to spin up a Grafana instance`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
