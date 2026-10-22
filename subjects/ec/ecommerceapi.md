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
- Valid runs: 1; wall time 48.4 to 48.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 75 | 48.4 | 5 | 5 | [run](https://argusic.com/run/1dccc02f-1abc-4319-80bf-419250dac06b) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `go: command not found; docker not installed`
- 5 min: `go build ./... failed: tests/e2e is package main without func main`
- 15 min: `No Postgres/Elasticsearch/Kafka binaries in the container`
- 20 min: `All five Go services hardcode port 8080, so they cannot run on one host without Docker`
- 6 min: `Python recommender pinned implicit==0.7.2 and requires-python <3.12`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
