# spotify-player

**Verdict: runs.** Argusic Score 86.2 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/aome510/spotify-player, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/spotify-player

## Pinned environment

- Project commit: `dac1fa7aa2c120cc67ead9e9c5c661ff017a2b94`
- Test commit: `dac1fa7aa2c120cc67ead9e9c5c661ff017a2b94`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, no run possible, run with mocked services
- Valid runs: 3; wall time 9.9 to 15.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 15 | 15.4 | 2 | 2 | [run](https://argusic.com/run/52e7b6a7-1ff8-427e-ab24-9c02360db83c) |
| 2 | fail | 66.67 | 14 | 9.9 | 3 | 1 | [run](https://argusic.com/run/df70f038-c298-4ebd-aadb-0528a0e637f7) |
| 3 | pass with mocks | 92 | 18 | 12.2 | 4 | 4 | [run](https://argusic.com/run/421961a3-b64f-4b12-871b-920192f5871f) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `rustc/cargo not installed`
- 4 min: `pkg-config could not find alsa/dbus-1 (no -dev headers, no root)`

Attempt 2:

- 1 min: `Rust toolchain not installed`
- `libasound2-dev missing (alsa.pc not found)`
- `libdbus-1-dev missing (dbus-1.pc not found)`

Attempt 3:

- 10 min: `Rust toolchain not installed (rustc: not found)`
- 4 min: `Linux dev packages libasound2-dev and libdbus-1-dev missing (no root)`
- 1 min: `Linker could not find libasound.so (dev .deb only shipped a symlink)`
- 1 min: `Linker failed on undefined symbols sd_listen_fds/sd_is_socket from static libdbus-1.a requiring libsystemd`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
