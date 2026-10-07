# openchoreo

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/openchoreo/openchoreo, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/openchoreo

## Pinned environment

- Project commit: `1aeed89856d088dc5160c0f3eaa39796d4a93611`
- Test commit: `1aeed89856d088dc5160c0f3eaa39796d4a93611`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 44.4 to 44.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 38 | 44.4 | 4 | 4 | [run](https://argusic.com/run/23985225-8f26-4c28-917c-dc6ed12c927c) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go 1.26.3 not found in container; project requires Go 1.26.x`
- 2 min: `Corrupted google.golang.org/protobuf module cache (NUL bytes in desc_validate.go) causing all Go packages importing protobuf to fail build`
- 1 min: `uv (Python package manager) not installed; Python agent tests cannot run without it`
- 2 min: `setup-envtest kubebuilder assets missing; controller tests hanging indefinitely`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
