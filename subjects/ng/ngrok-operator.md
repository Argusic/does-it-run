# ngrok-operator

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ngrok/ngrok-operator, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/ngrok-operator

## Pinned environment

- Project commit: `ca67b668abb77cf4d2fcaae4f55fe4ce8f34857c`
- Test commit: `ca67b668abb77cf4d2fcaae4f55fe4ce8f34857c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 8.2 to 8.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 8 | 8.2 | 2 | 2 | [run](https://argusic.com/run/16025db9-4cbd-4c48-a6af-20a6263c689c) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go 1.27 not installed in container`
- 1 min: `kubebuilder envtest binaries (etcd, kube-apiserver) not found at /usr/local/kubebuilder/bin/`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
