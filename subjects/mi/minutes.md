# minutes

**Verdict: runs.** Argusic Score 85 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/silverstein/minutes, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/minutes

## Pinned environment

- Project commit: `83531fa5bfc50192e9256263cf4d641b0ee50e7f`
- Test commit: `83531fa5bfc50192e9256263cf4d641b0ee50e7f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 29.9 to 29.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 85 | 29 | 29.9 | 4 | 1 | [run](https://argusic.com/run/daf3a00f-da17-4d9a-9ff4-4c33a5bc2a5f) |

## What was observed on a clean machine

Attempt 1:

- 10 min: `Missing system build dependencies: glib-2.0, libpipewire-0.3, libspa-0.2, alsa .pc files and headers for bindgen/libclang`
- `37 container-specific test failures in minutes-core: all use memfd_create or process-group operations (ENOSYS/os error 95) not available in this container`
- `1 container-specific test failure in minutes-cli test (authorized_process_fd): same operation-not-supported error`
- `12 MCP npm test failures: tests use import.meta.dirname (Node 21+) but container has Node 18`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
