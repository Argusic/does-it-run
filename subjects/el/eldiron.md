# Eldiron

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/markusmoenig/Eldiron, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/eldiron

## Pinned environment

- Project commit: `4b0908dc7eb37df588f70e71140119a4850290e0`
- Test commit: `4b0908dc7eb37df588f70e71140119a4850290e0`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 66.3 to 66.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 66 | 66.3 | 11 | 11 | [run](https://argusic.com/run/7d45057f-987b-4715-8b74-7270d658cddb) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Rust toolchain not found in container`
- 2 min: `alsa-sys build fails: pkg-config cannot find alsa.pc (no libasound2-dev)`
- 2 min: `wayland-sys build fails: pkg-config cannot find wayland-client.pc (no libwayland-dev)`
- 5 min: `yeslogic-fontconfig-sys build fails: missing fontconfig.pc (no libfontconfig-dev)`
- 1 min: `Linker: unable to find library -lasound (no .so symlink)`
- 1 min: `Linker: unable to find library -lwayland-client (broken .so symlink)`
- 1 min: `Linker: undefined XML_ParseBuffer etc from static libfontconfig.a needing libexpat`
- 3 min: `cargo check rusterix: cannot find type Widget (missing #[cfg(feature = "graphics")] gate on Widget::project_item_icon_frames call)`
- 2 min: `cargo test rusterix: PartyProbe missing 'say' method from WorldServices trait`
- 3 min: `GUI creator panics with AdapterNotFound (no Vulkan driver)`
- 2 min: `GUI creator panics at thedraw2d.rs:1828: index out of bounds during icon scaling`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
