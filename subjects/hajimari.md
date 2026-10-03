# hajimari

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/toboshii/hajimari, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/hajimari

## Pinned environment

- Project commit: `b07024d997942dcd97a533e89a92619d5a9cdd98`
- Test commit: `b07024d997942dcd97a533e89a92619d5a9cdd98`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 7.7 to 24.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 18 | 24.3 | 3 | 3 | [run](https://argusic.com/run/054793e7-1e5d-481b-960b-04cecc4e61fb) |
| 1 | pass | 100 | 8 | 7.7 | 1 | 1 | [run](https://argusic.com/run/ee6391b9-cf1d-4b1d-be0d-60ff613d72d3) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go not installed in container`
- 8 min: `No kubeconfig available - app requires Kubernetes connection`
- 1 min: `vet check failed: logrus.Error() has Printf formatting directive %s in crdapps/apps.go:72`

Attempt 1:

- 1 min: `internal/hajimari/crdapps/apps.go:72: logger.Error called with printf-style formatting directive instead of logger.Errorf`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
