# odigos

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/odigos-io/odigos, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/odigos

## Pinned environment

- Project commit: `ab65b465b4f8fabd8d8f83d91d6bff881be8ffcf`
- Test commit: `ab65b465b4f8fabd8d8f83d91d6bff881be8ffcf`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 27.5 to 27.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 7 | 27.5 | 3 | 3 | [run](https://argusic.com/run/5621e1f7-06d0-4959-b884-58b7763de092) |

## What was observed on a clean machine

Attempt 1:

- `Autoscaler tests require kubebuilder/etcd which is not available`
- `Collector configgrpc tests fail with gcController reference error`
- `k8sutils tests can't be discovered by 'go test' due to source files under pkg/ not at module root`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
