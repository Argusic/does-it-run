# k8ssandra-operator

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/k8ssandra/k8ssandra-operator, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/k8ssandra-operator

## Pinned environment

- Project commit: `2028d352ecb495de4b6e053d99d7a77b21eb5107`
- Test commit: `2028d352ecb495de4b6e053d99d7a77b21eb5107`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 38.2 to 38.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 1 | 38.2 | 6 | 6 | [run](https://argusic.com/run/27f18af6-ec35-4fb0-bfad-d84e38f945be) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Go not installed in container`
- 1 min: `kustomize not in PATH for tests`
- 2 min: `setup-envtest binary assets not installed`
- 1 min: `yq binary not found for test/yq tests`
- `controllers/k8ssandra, control, replication tests flaky: webhook race condition and 'too many open files' when running 3-4 envtest environments concurrently in this resource-constrained container`
- `controllers/replication consistently fails with 'too many open files' on manager start for data plane managers`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
