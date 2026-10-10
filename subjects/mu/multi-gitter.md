# multi-gitter

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/lindell/multi-gitter, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/multi-gitter

## Pinned environment

- Project commit: `b57d63b3c513078f26dad5c1b341e9505e9cad23`
- Test commit: `b57d63b3c513078f26dad5c1b341e9505e9cad23`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 40.1 to 40.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 2 | 40.1 | 5 | 5 | [run](https://argusic.com/run/f851c71b-ce77-49f1-8b0f-d0d5e7cea79d) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `no Go toolchain installed (go.mod requires go 1.26)`
- 1 min: `go build failed: could not create module cache at /root/go/pkg/mod (permission denied)`
- 42 min: `mock Gerrit smart-HTTP git endpoints and refs/for handling not wire-compatible with real git clients`
- 4 min: `first e2e run pushed but found no change (mock change row not created)`
- 2 min: `misread an earlier pre-fix failure as the final run's outcome`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
