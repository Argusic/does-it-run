# subtrace

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/subtrace/subtrace, licensed BSD-3-Clause, written in Go.

Evidence and recordings: https://argusic.com/subject/subtrace

## Pinned environment

- Project commit: `e3e3546b367ecc23d5fe5642491526ee969a6ff2`
- Test commit: `e3e3546b367ecc23d5fe5642491526ee969a6ff2`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 10.4 to 10.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 6 | 10.4 | 2 | 2 | [run](https://argusic.com/run/2293f17d-9511-439c-b0c8-92697d2ce3f2) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Go! language compiler (golang) not found in container`
- 1 min: `Test file cmd/run/fd/fd_test.go referred to renamed method IncRefLockForClose (now ClosingIncRef) and had type mismatch (bool vs nil)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
