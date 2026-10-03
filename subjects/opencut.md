# OpenCut

**Verdict: runs.** Argusic Score 94.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/OpenCut-app/OpenCut, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/opencut

## Pinned environment

- Project commit: `400f097becba5db0fbc305d5a65348cb81c20356`
- Test commit: `400f097becba5db0fbc305d5a65348cb81c20356`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 3; wall time 22.2 to 28.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 18.2 | 28.3 | 5 | 5 | [run](https://argusic.com/run/8766e389-5441-47ee-8c37-18aeac19f53e) |
| 2 | pass | 100 | 22 | 22.2 | 4 | 4 | [run](https://argusic.com/run/91607940-1d49-43dd-bf44-4f7b1373cac7) |
| 3 | pass | 92 | 27 | 27.2 | 5 | 3 | [run](https://argusic.com/run/d4355a87-3c22-4bfb-aaf3-8aadab4e88c9) |

## What was observed on a clean machine

Attempt 1:

- 5.5 min: `Missing .so symlinks for libxcb, libxkbcommon, libxkbcommon-x11 (only versioned .so.X files present, no .so symlinks for linker)`
- 3 min: `Rust sysroot lld linker could not find -lxcb, -lxkbcommon, -lxkbcommon-x11`
- 2 min: `Node.js v18.19.1 too old for Vite 8 (missing styleText export from node:util)`
- 2 min: `bun installer requires unzip (not available without root)`
- `Desktop app panics on GPU init: NoSupportedDeviceFound (no GPU in container)`

Attempt 2:

- 1 min: `cargo link failed: missing -lxcb, -lxkbcommon, -lxkbcommon-x11 (no .so symlinks for the linker)`
- 1 min: `web build failed: Node v18 lacks node:util.styleText export required by rolldown/vite 8`
- 2 min: `desktop binary panicked: NoSupportedDeviceFound (no Vulkan driver)`
- 1 min: `wrangler dev port 8787 Address already in use from previous run`

Attempt 3:

- 2 min: `Node.js 18.19.1 lacked 'styleText' export from 'node:util', required by rolldown (bundled via Vite 8)`
- 8 min: `Desktop release build failed: rust-lld could not find -lxcb, -lxkbcommon, -lxkbcommon-x11 (only .so.1/.so.0 existed, no bare .so symlinks)`
- 1 min: `Desktop binary panics on Xvfb: 'Failed to initialize X11 client' / 'NoSupportedDeviceFound' - no GPU available`
- `Web test suite (vitest) fails with 'depsOptimizer is required in dev mode' due to Cloudflare Vite plugin incompatibility`
- 1 min: `API wrangler dev failed on port 8787 (address already in use on first attempt)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
