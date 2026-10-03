# velero

**Verdict: runs with mocks.** Argusic Score 82 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/velero-io/velero, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/velero

## Pinned environment

- Project commit: `8e9f66addf6355d7f504f18d27b2841a3b2b8120`
- Test commit: `8e9f66addf6355d7f504f18d27b2841a3b2b8120`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 31.6 to 31.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 82 | 30.4 | 31.6 | 4 | 2 | [run](https://argusic.com/run/f8c18dd3-58ba-4d6f-a49f-30fff8b7f66d) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Go not installed in container`
- 8 min: `Go 1.26 vet: non-constant format string in Event/EndingEvent calls to EventRecorder`
- `pkg/controller test fails - needs envtest (etcd/kube-apiserver) binaries not present in container`
- `test/e2e and test/perf fail - need a real Kubernetes cluster, unavailable in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
