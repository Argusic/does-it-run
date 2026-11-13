# zapfast

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/crmne/zapfast, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/zapfast

## Pinned environment

- Project commit: `4497f08cee368235dedb4848990916bb40bfc88e`
- Test commit: `4497f08cee368235dedb4848990916bb40bfc88e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 64 to 75.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 74 | 75.3 | 4 | 4 | [run](https://argusic.com/run/803a3e57-1ad9-493c-a3bd-753e2861da06) |
| 2 | pass with mocks | 92 | 63 | 64 | 5 | 5 | [run](https://argusic.com/run/9242f2a5-92b4-4089-96b2-7966485aee19) |

## What was observed on a clean machine

Attempt 1:

- 10 min: `libpipewire-0.3-dev and libspa-0.2-dev not installed (no root), so pkg-config could not find libpipewire-0.3`
- 8 min: `libclang shared library missing for bindgen in libspa-sys build script`
- 3 min: `clang stdbool.h not found -- bindgen failed on pipewire version.h`
- 4 min: `ALSA pkg-config file missing and linker could not find -lasound`

Attempt 2:

- 1 min: `Rust toolchain 1.98.0 not installed`
- 5 min: `Missing system dev packages: libpipewire-0.3-dev, libspa-0.2-dev, libxkbcommon-dev, libwayland-dev, libxcb-*-dev, libasound2-dev, libpango1.0-dev, x11proto-dev, libxau-dev, libxdmcp-dev`
- 2 min: `libclang (libclang1-18, libclang-18-dev) needed for bindgen`
- 1 min: `libLLVM.so.18.1 needed by libclang at runtime`
- 1 min: `Linker could not find libpipewire-0.3.so and libasound.so (no -dev symlinks to unversioned .so)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
