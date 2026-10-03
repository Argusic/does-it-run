# mm-wiki

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/phachon/mm-wiki, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/mm-wiki

## Pinned environment

- Project commit: `d976d0c604847503bfcea2829489ce278e2c6cf7`
- Test commit: `d976d0c604847503bfcea2829489ce278e2c6cf7`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 45.6 to 45.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 15 | 45.6 | 4 | 4 | [run](https://argusic.com/run/36295279-8a55-4797-9d32-1e0cbe32269c) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go not installed in container`
- 5 min: `MariaDB not installed in container`
- 3 min: `Database schema not set up`
- `2 pre-existing test failures in app/utils (zipx_test.go use hardcoded developer paths)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
