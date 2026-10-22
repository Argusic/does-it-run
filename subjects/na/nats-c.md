# nats.c

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/nats-io/nats.c, licensed Apache-2.0, written in C.

Evidence and recordings: https://argusic.com/subject/nats-c

## Pinned environment

- Project commit: `a0777d6daa4fb695f9dfd35901b7b734d3845bb2`
- Test commit: `a0777d6daa4fb695f9dfd35901b7b734d3845bb2`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 14.4 to 14.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 18 | 14.4 | 3 | 3 | [run](https://argusic.com/run/7caacfa5-52a0-41f4-82da-466a6f1cfcaf) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `make install lacked permissions to write to /usr/local/lib/pkgconfig (no root in container)`
- 4 min: `Tests IPResolutionOrder and natsSock_IPOrder failed: IPv6-only checks cannot pass because the container has IPv6 disabled`
- 4 min: `Brand-new test suite lacks a nats-server binary, which tests fork via execvp`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
