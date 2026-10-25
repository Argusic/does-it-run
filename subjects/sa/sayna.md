# sayna

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/SaynaAI/sayna, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/sayna

## Pinned environment

- Project commit: `2be27ae0b8acf7d53fc574588e8a8ad0bb60ce09`
- Test commit: `2be27ae0b8acf7d53fc574588e8a8ad0bb60ce09`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 19.1 to 19.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 8 | 19.1 | 6 | 6 | [run](https://argusic.com/run/5f425f59-40a3-4d0a-9b72-7ed9599c6503) |

## What was observed on a clean machine

Attempt 1:

- 0.25 min: `Rust toolchain not installed`
- 3 min: `glib-sys build failure: glib-2.0.pc not found (libglib2.0-dev not installed)`
- 1 min: `webrtc-sys build failure: missing libdrm.pc, gbm.pc`
- 2 min: `webrtc-sys build failure: missing X11 dev packages (x11, xfixes, xdamage, xrandr, xcomposite, xext, xcb, xau, xdmcp)`
- 0.5 min: `webrtc-sys build failure: missing libva-dev, libvdpau-dev, libpciaccess-dev`
- 1 min: `Linker error: static libX11.a pulled in with unresolved xcb symbols`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
