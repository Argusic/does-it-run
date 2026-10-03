# milvus

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/milvus-io/milvus, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/milvus

## Pinned environment

- Project commit: `15fdc95998549f6508c29b14671e2aad37db1ee4`
- Test commit: `15fdc95998549f6508c29b14671e2aad37db1ee4`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 31.2 to 31.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 30 | 31.2 | 5 | 5 | [run](https://argusic.com/run/5fe1fdd1-7b82-4cb5-9db5-a2f8a02ceeb9) |

## What was observed on a clean machine

Attempt 1:

- 10 min: `Go not found in container`
- 5 min: `PEP 668 blocks system pip for pymilvus and conan install`
- 5 min: `Full C++ source build (make) fails , Conan needs root-installed system packages (libaio, etc.) and 30+ min compile`
- `10 Go packages fail to build: rocksdb, rdkafka, pulsar C libs not in container`
- `10 Go packages fail tests: paramtable/indexparams/tracer/interceptor/lock/nodescheduler/wp panic on mkdir /var/lib/milvus (permission denied); config flakes on etcd port conflict; pulsar needs running server`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
