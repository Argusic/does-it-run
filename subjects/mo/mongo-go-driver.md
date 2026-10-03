# mongo-go-driver

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/mongodb/mongo-go-driver, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/mongo-go-driver

## Pinned environment

- Project commit: `74620faf2f7b960417e8d590acf3f9b0d4e00b80`
- Test commit: `74620faf2f7b960417e8d590acf3f9b0d4e00b80`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 6.4 to 6.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 6.5 | 6.4 | 3 | 3 | [run](https://argusic.com/run/b8562621-4362-439a-83c5-7a4538a86ceb) |

## What was observed on a clean machine

Attempt 1:

- 2.5 min: `Go 1.26 not found in PATH`
- 4 min: `Git submodules not initialized (testdata/specifications missing)`
- 0.5 min: `Test failure in internal/handshake/operation: container metadata detection adds 'runtime:docker' field not expected by test`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
