# diri

**Verdict: runs.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/cristicretu/diri, licensed AGPL-3.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/diri

## Pinned environment

- Project commit: `1a8e9d96091b3ea2db5821d3da9cbe97e7140033`
- Test commit: `1a8e9d96091b3ea2db5821d3da9cbe97e7140033`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 34.1 to 34.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 92 | 18 | 34.1 | 5 | 3 | [run](https://argusic.com/run/23f60ac9-f999-49a1-b98d-2c9d816383d5) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Missing system -dev packages (libasound2-dev, libfontconfig-dev, libglib2.0-dev, libwayland-dev, libx11-xcb-dev, libxkbcommon-dev, libxkbcommon-x11-dev, libfreetype-dev, zlib1g-dev, libpng-dev, libbrotli-dev, libexpat1-dev, libxcb1-dev) , n`
- 1 min: `Dangling symlinks in build-deps (libxcb.so.0, libxkbcommon.so.0, libxkbcommon-x11.so.0) caused linker errors`
- 1 min: `Missing field foreground_ports in SessionView test initializer at crates/diri-engine/src/registry.rs:5048`
- `3 pre-existing test failures in control::claude_accounts and control::codex_accounts , credential file permission checks fail in this container environment (also fail on unmodified code)`
- `Full desktop binary linking (diri-app) runs out of memory in 8GB container , cargo check succeeds but final ld OOMs`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
