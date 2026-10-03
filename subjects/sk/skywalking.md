# skywalking

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/apache/skywalking, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/skywalking

## Pinned environment

- Project commit: `0a01d89d333ff08535b3630a38ef45fc0dcbca10`
- Test commit: `0a01d89d333ff08535b3630a38ef45fc0dcbca10`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 37 to 55.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 55.1 | 0 | 0 | [run](https://argusic.com/run/c557f33e-a01e-475c-8f2d-fdf15115129a) |
| 2 | pass | 100 | 20 | 37 | 5 | 5 | [run](https://argusic.com/run/55a33bc8-20b9-4828-acf1-610b4c5ac26a) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `No JDK installed in container`
- `Missing JDK 17+ and Maven 3.6+`
- 1 min: `Git submodules not initialized (apm-protocol, banyandb-client-proto, query-protocol)`
- `Maven install failed due to missing gpg binary for signing`
- 3 min: `OAP server failed to start - default storage is BanyanDB (external service, not running)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
