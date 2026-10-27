# aperture

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/fluxninja/aperture, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/run/9fcac26b-c7ea-4113-bfb0-96ed906a9b1a

## Pinned environment

- Project commit: `6b5320ab674cfb03f0f13b6c7714f998a0526bdc`
- Test commit: `6b5320ab674cfb03f0f13b6c7714f998a0526bdc`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 35.2 to 35.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 23.6 | 35.2 | 9 | 9 | [run](https://argusic.com/run/9fcac26b-c7ea-4113-bfb0-96ed906a9b1a) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `No Go toolchain in container`
- 2 min: `No etcd binary available`
- 3 min: `No prometheus binary available`
- 1 min: `gotestsum not found`
- 3 min: `GNU parallel not found`
- 1 min: `Agent/controller port conflict on :8080`
- 2 min: `OTel collector port collisions (zpages/pprof/health ports shared between controller and agent)`
- 1 min: `Prometheus remote-write endpoint returning 404`
- 1 min: `Operator tests require kubebuilder envtest binaries (etcd and kube-apiserver) which need GCS access (401 Unauthorized)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
