# tplay

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/maxcurzi/tplay, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/tplay

## Pinned environment

- Project commit: `c62dca0da1696e57eb9726cfe08354311587fb7f`
- Test commit: `c62dca0da1696e57eb9726cfe08354311587fb7f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 26.3 to 26.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 26 | 26.3 | 5 | 5 | [run](https://argusic.com/run/0b491d7e-3669-443b-ae4f-9613854f8e59) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `Rust toolchain and FFmpeg/mpv dev headers absent (no root); pkg-config found no libavformat`
- 13 min: `ffmpeg-sys-next hit 'libavformat not found' then 'limits.h not found' during bindgen`
- 6 min: `ld picked broken static archives; undefined MFX/OpenCL symbols`
- 4 min: `binary failed at runtime: libdvdnav/libmujs/liblua5.2/libsixel/libXpresent/libva-wayland missing`
- 1 min: `yt-dlp Debian wrapper needs its dist-packages`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
