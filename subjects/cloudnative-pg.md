# cloudnative-pg

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/cloudnative-pg/cloudnative-pg, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/cloudnative-pg

## Pinned environment

- Project commit: `c60ac252f566131b6988943d2093825481759fd7`
- Test commit: `c60ac252f566131b6988943d2093825481759fd7`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 15.9 to 15.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 10.2 | 15.9 | 1 | 1 | [run](https://argusic.com/run/353bad74-b891-4309-8f34-b222a852c5e9) |

## What was observed on a clean machine

Attempt 1:

- 3.5 min: `Missing kubebuilder binaries (kube-apiserver, etcd) for envtest in internal/cmd/plugin`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
