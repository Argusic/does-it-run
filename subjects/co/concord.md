# concord

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Cogmasters/concord, licensed MIT, written in C.

Evidence and recordings: https://argusic.com/subject/concord

## Pinned environment

- Project commit: `fb0f834d07d65048a6afde177e318fe9659a9494`
- Test commit: `fb0f834d07d65048a6afde177e318fe9659a9494`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 17.7 to 17.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 0.5 | 17.7 | 2 | 2 | [run](https://argusic.com/run/cb2054dc-320b-4d18-920b-44cb24034fe4) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Missing libcurl4-openssl-dev (curl/curl.h header) , the deb package is not installed in the container and the build breaks at core/io_poller.c:5`
- 1 min: `Gencodecs stale output , if gencodecs/Makefile runs after a prior crash, leftover discord_codecs.c/h are truncated and fail with unterminated #ifndef`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
