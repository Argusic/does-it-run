# ggez

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ggez/ggez, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/ggez

## Pinned environment

- Project commit: `9c865474504084b60204874bc028ba91c5f013b9`
- Test commit: `9c865474504084b60204874bc028ba91c5f013b9`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 9.5 to 19.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 18.2 | 19.4 | 7 | 7 | [run](https://argusic.com/run/d6c34a1e-32b4-432a-8e34-5839ca96473b) |
| 2 | pass with mocks | 92 | 3.5 | 9.5 | 4 | 4 | [run](https://argusic.com/run/b2a93ad9-79c1-436e-b5b5-6c83dfd63b71) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Rust toolchain not installed`
- 2 min: `alsa-sys build failure: missing libasound2-dev headers/pkg-config`
- 1.5 min: `libudev-sys build failure: missing libudev-dev`
- 2 min: `Audio initialization fails at runtime (no ALSA hardware)`
- 3 min: `Vulkan ICD missing , graphics initialization failure`
- 1 min: `Missing libEGL.so and libGLESv2.so symlinks`
- 1 min: `context::tests::has_traits fails: winit rejects event loop on non-main thread (cargo test uses thread pool)`

Attempt 2:

- 1.5 min: `Missing system -dev packages (alsa, x11, xcb, xkbcommon, vulkan, egl, udev headers) prevented compilation`
- 0.1 min: `Runtime .so symlinks (libudev.so, libasound.so) missing for linker`
- `context::tests::has_traits test fails: AudioError from no audio hardware in container`
- `Examples fail to run: AudioError (with audio) or GraphicsInitializationError (without audio) due to no GPU/audio hardware`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
