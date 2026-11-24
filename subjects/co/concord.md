# concord

**Verdict: runs with mocks.** Argusic Score 89.5 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Cogmasters/concord, licensed MIT, written in C.

Evidence and recordings: https://argusic.com/subject/concord

## Pinned environment

- Project commit: `fb0f834d07d65048a6afde177e318fe9659a9494`
- Test commit: `fb0f834d07d65048a6afde177e318fe9659a9494`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 17.2 to 17.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 0.5 | 17.7 | 2 | 2 | [run](https://argusic.com/run/cb2054dc-320b-4d18-920b-44cb24034fe4) |
| 2 | pass with mocks | 87 | 18 | 17.2 | 4 | 3 | [run](https://argusic.com/run/f57aeec4-9d74-49dd-8a85-42401c872a96) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Missing libcurl4-openssl-dev (curl/curl.h header) , the deb package is not installed in the container and the build breaks at core/io_poller.c:5`
- 1 min: `Gencodecs stale output , if gencodecs/Makefile runs after a prior crash, leftover discord_codecs.c/h are truncated and fail with unterminated #ifndef`

Attempt 2:

- 6 min: `curl/curl.h missing (libcurl4-openssl-dev not installed, no root)`
- 5 min: `test Makefile overrides CFLAGS/LDFLAGS so curl headers/libs not found; static libcurl.a loses DES/GSS symbols`
- 7 min: `Discord tests fail 401 against real API (placeholder token); gateway tests need live websocket`
- `websockets test requires autobahn fuzzingserver (pip2 unavailable)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
