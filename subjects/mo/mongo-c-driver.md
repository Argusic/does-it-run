# mongo-c-driver

**Verdict: runs.** Argusic Score 93.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/mongodb/mongo-c-driver, licensed Apache-2.0, written in C.

Evidence and recordings: https://argusic.com/subject/mongo-c-driver

## Pinned environment

- Project commit: `4ce399222e21a08cfdb57eeef92edd6f2fd2f32c`
- Test commit: `4ce399222e21a08cfdb57eeef92edd6f2fd2f32c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 22.8 to 22.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 93.33 | 15 | 22.8 | 3 | 2 | [run](https://argusic.com/run/24bb47aa-e758-42ad-969b-467d2fdc065d) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `cmake --install failed: libbson2.so.2.6.0 missing (only test target had been built)`
- 10 min: `7 crud/unified *-errorResponse tests failed: no such command 'configureFailPoint' (mongod started without test commands)`
- 5 min: `3 Client tests fail: /Client/ipv6/single, /Client/ipv6/pooled (no IPv6 in container; cannot reach [::1]:27017) and /Client/ssl/reconnect/pooled (expects 'Failed to buffer 4 bytes' log line not emitted)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
