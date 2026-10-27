# solr-operator

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/apache/solr-operator, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/solr-operator

## Pinned environment

- Project commit: `ed5c5c7d28a4c1189d19f581259e05385c0d4b20`
- Test commit: `ed5c5c7d28a4c1189d19f581259e05385c0d4b20`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 11.8 to 11.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 10.8 | 11.8 | 2 | 2 | [run](https://argusic.com/run/e611761c-0287-45a5-905b-d3b08c860ba9) |

## What was observed on a clean machine

Attempt 1:

- 1.5 min: `Go 1.27.3 not installed on system`
- 6 min: `kubebuilder envtest binaries (etcd, kube-apiserver) not found at /usr/local/kubebuilder/bin/`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
