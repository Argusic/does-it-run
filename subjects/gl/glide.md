# glide

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/philn/glide, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/glide

## Pinned environment

- Project commit: `b8f1c7c972278ec7e6041c1b6b1319faa643321b`
- Test commit: `b8f1c7c972278ec7e6041c1b6b1319faa643321b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 21.9 to 21.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 20 | 21.9 | 5 | 5 | [run](https://argusic.com/run/7dc86b3f-c0b1-4874-9c73-b632f95bf0ea) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Rust toolchain missing`
- 12 min: `Missing system dev libraries for glib, gstreamer, gtk4, libadwaita, etc.`
- 1 min: `Missing GStreamer plugin libraries for playbin/playback element`
- 1 min: `Missing D-Bus session bus (app requires MPRIS server)`
- 1 min: `Missing ffmpeg/libav runtime libraries for gstreamer codecs`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
