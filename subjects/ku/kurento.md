# kurento

**Verdict: could not verify.** Argusic Score 20 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Kurento/kurento, licensed Apache-2.0, written in C.

Evidence and recordings: https://argusic.com/subject/kurento

## Pinned environment

- Project commit: `2e4bf5524ac4fde5d58071344a103429b5901f85`
- Test commit: `2e4bf5524ac4fde5d58071344a103429b5901f85`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, no run possible
- Valid runs: 2; wall time 7.5 to 16.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | 15 | 16.3 | 4 | 4 | [run](https://argusic.com/run/be925357-2c0e-41e1-abfb-001d7cd3c68f) |
| 2 | fail | 20 | n/a | 7.5 | 0 | 0 | [run](https://argusic.com/run/568bff5a-e34b-4c11-ab1a-f8b6a968e51a) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Java/Maven not pre-installed`
- 1 min: `jsoncpp-dev headers missing for C++ build`
- 3 min: `Boost development packages missing`
- 5 min: `C++ server requires ~30 system -dev packages (gstreamer, glib, libnice, libffi, libpcre2, libunwind, libelf, libdw, zlib, etc.)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
