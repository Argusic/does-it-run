# kube-state-metrics

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/kubernetes/kube-state-metrics, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/kube-state-metrics

## Pinned environment

- Project commit: `f77f1b8c3bb7ffc6e5cfa7872a81c8f67b567e2c`
- Test commit: `f77f1b8c3bb7ffc6e5cfa7872a81c8f67b567e2c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 8.8 to 8.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 7.5 | 8.8 | 2 | 2 | [run](https://argusic.com/run/5e857899-fdf0-4199-a66d-4e7bc067af5b) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go compiler not found in container`
- 3 min: `e2e tests (TestAuthFilter, TestCRDInformerUpdateFuncHandler) need a real Kubernetes cluster with kubectl`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
