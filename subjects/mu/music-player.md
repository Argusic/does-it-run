# music-player

**Verdict: runs.** Argusic Score 98.8 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/tsirysndr/music-player, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/music-player

## Pinned environment

- Project commit: `1658a2b247a82f4945a29e2abcfe1b7149567b5d`
- Test commit: `1658a2b247a82f4945a29e2abcfe1b7149567b5d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 45.9 to 46.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 97.5 | 14.5 | 45.9 | 8 | 7 | [run](https://argusic.com/run/cd2a2e6a-583b-42e7-adb6-799b50cc7e8a) |
| 2 | pass | 100 | 18 | 46.5 | 3 | 3 | [run](https://argusic.com/run/d596eeda-45c3-41e3-8bf7-80320082877e) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `alsa-sys build failed: libasound2-dev not installed`
- 2 min: `protoc not found for grpc build`
- 1 min: `Linker cannot find libasound.so`
- `souvlaki/zbus MPRIS panic on startup (no D-Bus in container)`
- 2 min: `playback tests failed: no ALSA device (cpal default)`
- 1 min: `Scanner test failed: /tmp/audio symlinks not set up`
- 2 min: `Settings test failed: config values mismatched defaults`
- `glib-sys build failed for desktop crate (no glib-2.0-dev)`

Attempt 2:

- 2 min: `ALSA dev headers (libasound2-dev) not found , pkg-config cannot find alsa.pc`
- 1 min: `protoc compiler not found , prost-build requires it for gRPC codegen`
- 3 min: `playback integration tests fail , default OutputConfig::Cpal unsupported without cpal`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
