# function-mesh

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/streamnative/function-mesh, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/function-mesh

## Pinned environment

- Project commit: `a2cb1ca50b63385e2ded8f7b2a2bd1bcc4011462`
- Test commit: `a2cb1ca50b63385e2ded8f7b2a2bd1bcc4011462`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 7.7 to 7.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1.5 | 7.7 | 2 | 2 | [run](https://argusic.com/run/db716652-3692-47d9-ab7b-b4bad3ff1f5b) |

## What was observed on a clean machine

Attempt 1:

- 1.5 min: `No Go compiler found in environment`
- 0.5 min: `envtest binaries missing at /usr/local/kubebuilder/bin/ (etcd, kube-apiserver, kubectl)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
