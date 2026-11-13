# gnvim

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/vhakulinen/gnvim, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/gnvim

## Pinned environment

- Project commit: `38b1037d90c9c024f0eab45f703d15a9ebd6e863`
- Test commit: `38b1037d90c9c024f0eab45f703d15a9ebd6e863`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 15.1 to 20.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 19 | 20.3 | 0 | 0 | [run](https://argusic.com/run/f56308e4-2931-4716-ae3e-821946d4279f) |
| 2 | pass | 100 | 12.5 | 15.1 | 6 | 6 | [run](https://argusic.com/run/4062842d-b501-46e7-93a8-62936fcc1031) |

## What was observed on a clean machine

Attempt 2:

- 8 min: `No Rust toolchain, GTK4/libadwaita dev packages, or Neovim available in the container`
- 1 min: `cargo build failed: glib-build-tools build script could not find glib-compile-resources`
- 1 min: `libappstream.so.5 and libxmlb.so.2 missing from dev dir at runtime`
- 0.5 min: `libyaml-0.so.2 missing at runtime`
- 1.5 min: `nvim binary (0.9.5 from apt) too old , README requires 0.10+, API not compatible`
- 0.5 min: `GSettings schema 'com.github.vhakulinen.gnvim.Devel' not installed`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
