# k8s

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Thakurvaibhav/k8s, licensed MIT, written in Shell.

Evidence and recordings: https://argusic.com/subject/k8s

## Pinned environment

- Project commit: `b36530262a20f68245d6b60ad35eecc63aa3c79a`
- Test commit: `b36530262a20f68245d6b60ad35eecc63aa3c79a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 44.5 to 44.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 42 | 44.5 | 5 | 5 | [run](https://argusic.com/run/8f2d3e78-4179-427d-a7a6-f8f58c59ca66) |

## What was observed on a clean machine

Attempt 1:

- 6 min: `Missing required binaries (helm, yq, trivy, checkov)`
- 3 min: `cert-manager Helm dependency resolution failed - repo mismatch against Chart.yaml versions v1.16.3 and reflector 7.1.262`
- 13 min: `scripts/scan.sh debug() function uses (( DEBUG )) arithmetic which returns exit code 1 with set -e when DEBUG=0, killing the entire scan silently`
- 2 min: `Missing helm repos for eck-operator, elastic-stack, envoy-gateway, external-dns, jaeger, kyverno, redis, sealed-secrets, valkey`
- `checkov scan reports 4 failures for kyverno chart (CPU/memory limits on upstream dependency templates)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
