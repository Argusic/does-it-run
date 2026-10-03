# badger

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/dgraph-io/badger, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/badger

## Pinned environment

- Project commit: `5688f1406cedb8e7cd22401855a90ad6b9ce733c`
- Test commit: `5688f1406cedb8e7cd22401855a90ad6b9ce733c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 11.3 to 11.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.5 | 11.3 | 4 | 4 | [run](https://argusic.com/run/b2b8b232-275e-454a-b6f9-9896d327fa5e) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `Go not installed in container`
- `go test -race OOM on TestSyncForRace`
- `pb.TestProtosRegenerate fails: protoc not installed`
- `jemalloc tag build fails: jemalloc/jemalloc.h missing`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
