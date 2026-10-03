# concourse

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/concourse/concourse, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/concourse

## Pinned environment

- Project commit: `d6e25a33812ac30a9e097fc547b93a2f48040bdc`
- Test commit: `d6e25a33812ac30a9e097fc547b93a2f48040bdc`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 81.2 to 81.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 45 | 81.2 | 5 | 5 | [run](https://argusic.com/run/10be21b0-7487-4c38-8432-3498d3c8bde4) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go compiler not pre-installed`
- 2 min: `yarn not pre-installed and npm install -g blocked by permissions`
- 3 min: `initdb/postgres binaries not available for test suite`
- 1 min: `Postgres JIT loader fails with missing libLLVM-17.so.1`
- 20 min: `Elm test suite (3095 tests) spawns 192 parallel workers (equal to CPU count), causing socket IPC failures`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
