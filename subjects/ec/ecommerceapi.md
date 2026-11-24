# EcommerceAPI

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/rasadov/EcommerceAPI, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/ecommerceapi

## Pinned environment

- Project commit: `6f2d32bfed0fb24fbed4c52cd5688b5a24904543`
- Test commit: `6f2d32bfed0fb24fbed4c52cd5688b5a24904543`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 10.9 to 48.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 75 | 48.4 | 5 | 5 | [run](https://argusic.com/run/1dccc02f-1abc-4319-80bf-419250dac06b) |
| 2 | pass with mocks | 92 | 10 | 10.9 | 4 | 4 | [run](https://argusic.com/run/4a416fd1-bf41-4e2f-937e-d95638d58e30) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `go: command not found; docker not installed`
- 5 min: `go build ./... failed: tests/e2e is package main without func main`
- 15 min: `No Postgres/Elasticsearch/Kafka binaries in the container`
- 20 min: `All five Go services hardcode port 8080, so they cannot run on one host without Docker`
- 6 min: `Python recommender pinned implicit==0.7.2 and requires-python <3.12`

Attempt 2:

- 2 min: `Python recommender circular import: shared/db/repo.py imported from recommendations.weights which triggered a circular chain back to shared/db/repo`
- 4 min: `Go 1.23 not installed in container; had to download and install manually`
- `Docker not available in container; full stack (Kafka, PostgreSQL, Elasticsearch) cannot run`
- `No PostgreSQL/Kafka/Elasticsearch services running; e2e tests require full Docker stack`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
