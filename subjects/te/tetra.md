# tetra

**Verdict: runs.** Argusic Score 90 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/17cupsofcoffee/tetra, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/tetra

## Pinned environment

- Project commit: `b3ce706f8275609be4f91ddedfa484b657e2ae43`
- Test commit: `b3ce706f8275609be4f91ddedfa484b657e2ae43`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 8.1 to 13.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 6 | 8.1 | 2 | 2 | [run](https://argusic.com/run/3c8ce733-16d2-4155-9f5f-e68fae161c45) |
| 2 | pass | 100 | 8 | 13.2 | 3 | 3 | [run](https://argusic.com/run/4af7e545-05cd-4ee2-9ec2-7f06df397d5c) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `SDL3 build-from-source failed: CMake requires X11 or Wayland dev headers on Linux.`
- 1 min: `alsa-sys build failed: pkg-config cannot find alsa.pc (libasound2-dev headers missing).`

Attempt 2:

- 1 min: `alsa-sys failed: libasound2-dev not installed (no root)`
- 1 min: `Linker: -lSDL3 not found (no system SDL3)`
- 2 min: `SDL cmake: missing X11/Wayland dev headers`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
