# mimi

**Verdict: runs with mocks.** Argusic Score 87 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/yuxino/mimi, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/run/c9f8c2e6-78e0-4014-ad11-0611c30837db

## Pinned environment

- Project commit: `9eae2b87be8092a92dc5bca98b793d1e36917b10`
- Test commit: `9eae2b87be8092a92dc5bca98b793d1e36917b10`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 21.1 to 21.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 87 | 21 | 21.1 | 4 | 3 | [run](https://argusic.com/run/c9f8c2e6-78e0-4014-ad11-0611c30837db) |

## What was observed on a clean machine

Attempt 1:

- `Node.js v18 installed (needs ^20.19.0) - engine check warned but all commands succeeded`
- 1 min: `Rust toolchain not installed`
- 15 min: `Missing system -dev libraries (no root) - webkit2gtk, GTK3, GLib, libsoup, X11 protos`
- 3 min: `Linker failed to find system .so files at link time`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
