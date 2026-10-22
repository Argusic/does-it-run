# cyberapi

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/vicanso/cyberapi, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/cyberapi

## Pinned environment

- Project commit: `5b959b8f33d8e58b627427b08566a7069b3792ad`
- Test commit: `5b959b8f33d8e58b627427b08566a7069b3792ad`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 66.6 to 66.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 38 | 66.6 | 5 | 5 | [run](https://argusic.com/run/2be3f97c-6977-4812-b548-c187c7cf4e80) |

## What was observed on a clean machine

Attempt 1:

- 6 min: `yeslogic-fontconfig-sys build failed: no fontconfig dev headers/.pc to compile bindings`
- 4 min: `linker: unable to find -lxkbcommon, -lxkbcommon-x11, -lxcb (runtime .so.0s present, no dev symlinks, no root for apt)`
- 3 min: `cargo test: this_build::tests::the_desktop_reads_files panicked on missing Downloads/XDG user dirs in container`
- 14 min: `first launch showed startup-error window and wrote no DB: data dir parent absent and turso does not create it`
- 8 min: `disk filled (40G) by two full build+test passes; sqlx bridge test build failed with No space left on device`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
