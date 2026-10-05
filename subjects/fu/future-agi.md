# future-agi

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/future-agi/future-agi, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/future-agi

## Pinned environment

- Project commit: `ec05d596da5627bf844cc22640790a2f85d6a48b`
- Test commit: `ec05d596da5627bf844cc22640790a2f85d6a48b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 50.2 to 50.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 49 | 50.2 | 4 | 4 | [run](https://argusic.com/run/e29d078a-c6ee-4dc2-994f-6cf3c840e464) |

## What was observed on a clean machine

Attempt 1:

- `No Docker daemon available - required for the standard install (docker compose)`
- `Node.js v18.19.1 installed, but frontend requires >=22.18.0`
- `Frontend test: 1 performance test fails with timing flake - expected duration <200ms but got ~365ms in this container`
- `Backend tests require Docker-based test infrastructure (PostgreSQL, ClickHouse, Redis, MinIO via docker-compose.test.yml) - cannot run without it`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
