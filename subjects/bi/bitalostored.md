# bitalostored

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/zuoyebang/bitalostored, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/bitalostored

## Pinned environment

- Project commit: `6150692f5a7991115c461b7f54e60fa8b8c2b5ed`
- Test commit: `6150692f5a7991115c461b7f54e60fa8b8c2b5ed`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 56.1 to 56.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 38 | 56.1 | 6 | 6 | [run](https://argusic.com/run/132f00c6-120e-4edd-a150-0f1063d2f73a) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `go toolchain missing in container`
- 9 min: `makefile bitalostored link fails: ld cannot find -lz -lbz2 -lsnappy -llz4 (no root for apt)`
- 6 min: `go test ./stored/cmd_test and large test batches OOM-killed (1.9GB container; single-node db ~1.5GB RSS)`
- 7 min: `TestKeysCmds flaky: pttl err 1831-1832 (raft pause drifts PTTL clock)`
- 3 min: `TestClusterReplication first run redigo nil returned`
- 1 min: `GET/LRANGE/SCARD and COMMAND return ERR invalid bulk length from main loop`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
