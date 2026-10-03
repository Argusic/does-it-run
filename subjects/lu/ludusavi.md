# ludusavi

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/mtkennerly/ludusavi, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/ludusavi

## Pinned environment

- Project commit: `70f4abb31497fa5ed9b0d24098200f3662d6fda9`
- Test commit: `70f4abb31497fa5ed9b0d24098200f3662d6fda9`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 26.6 to 26.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 20 | 26.6 | 6 | 6 | [run](https://argusic.com/run/1fdf9597-1e95-474a-a742-cb699bba82bb) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `rustc not found`
- 3 min: `glib-sys build failure: glib-2.0.pc missing`
- 4 min: `gio-sys build failure: transitive pkg-config missing (zlib, mount, libselinux)`
- 5 min: `gdk-sys build failure: deeper transitive pkg-config chain broken`
- 1 min: `linker: unable to find -lgtk-3, -lgdk-3, etc`
- `GUI: MESA shm/DRI3 errors on Xvfb`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
