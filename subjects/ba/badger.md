# badger

**Verdict: runs.** Argusic Score 96.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/dgraph-io/badger, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/badger

## Pinned environment

- Project commit: `5688f1406cedb8e7cd22401855a90ad6b9ce733c`
- Test commit: `5688f1406cedb8e7cd22401855a90ad6b9ce733c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 11.3 to 19.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.5 | 11.3 | 4 | 4 | [run](https://argusic.com/run/b2b8b232-275e-454a-b6f9-9896d327fa5e) |
| 2 | pass | 93.33 | 19 | 19.8 | 3 | 2 | [run](https://argusic.com/run/669265d5-f2b9-460c-ac14-2393fe2bb21f) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `Go not installed in container`
- `go test -race OOM on TestSyncForRace`
- `pb.TestProtosRegenerate fails: protoc not installed`
- `jemalloc tag build fails: jemalloc/jemalloc.h missing`

Attempt 2:

- 2 min: `Go 1.24.3 not installed in container`
- 10 min: `jemalloc not installed; ristretto v2.2.0 hardcodes LDFLAGS to /usr/local/lib (unwritable)`
- `pb/TestProtosRegenerate fails: protoc (protobuf compiler) not found`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
