# spicedb

**Verdict: runs.** Argusic Score 90.8 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/authzed/spicedb, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/spicedb

## Pinned environment

- Project commit: `9145a33f9a092d3420be8469cb88f5ac30b16bc2`
- Test commit: `9145a33f9a092d3420be8469cb88f5ac30b16bc2`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 15.9 to 26.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 86.67 | 15 | 15.9 | 3 | 1 | [run](https://argusic.com/run/12a6c304-9361-48c1-85b8-377172e026da) |
| 2 | pass | 95 | 26 | 26.3 | 4 | 3 | [run](https://argusic.com/run/4f88cd42-b722-4611-a024-3109efdea706) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go 1.26 not installed in container`
- 5 min: `pkg/cmd tests fail: requires Docker for CockroachDB testcontainer (rootless Docker not found)`
- 5 min: `pkg/testutil/sdbtestcontainer tests fail: requires Docker for SpiceDB testcontainer (rootless Docker not found)`

Attempt 2:

- 5 min: `No Go toolchain in container`
- 3 min: `README 'serve' example flags (--grpc-no-tls/--http-no-tls) and plain-HTTP start not valid for HTTP without TLS certs`
- 16 min: `Full mage test:unit run hung ~16 min in cache-missed internal/services/v1 run under 4-core/768MB container (stream-timeout goroutine)`
- 2 min: `Datastore tests fail: rootless Docker not found (sdbtestcontainer, pkg/cmd GC/repair/migrate) and e2e needs cockroach binary`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
