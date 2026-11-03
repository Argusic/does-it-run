# wordcraft

**Verdict: runs.** Argusic Score 98.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/storytold/wordcraft, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/wordcraft

## Pinned environment

- Project commit: `37318985b570527bad2c5d908dd2e718609585fc`
- Test commit: `37318985b570527bad2c5d908dd2e718609585fc`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 38.3 to 71.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 68 | 71.7 | 1 | 1 | [run](https://argusic.com/run/e04ea0af-98f0-43b9-9011-969345088d4c) |
| 2 | pass | 96.67 | 9 | 38.3 | 6 | 5 | [run](https://argusic.com/run/59222233-9530-4a70-a094-245e19329d43) |

## What was observed on a clean machine

Attempt 1:

- `3 pre-existing layout test failures`

Attempt 2:

- 8 min: `No Rust toolchain installed; rustup 1.90.0 then failed with 'rustc 1.90.0 is not supported by eframe/egui 0.36.2 (requires 1.95)' despite workspace rust-version 1.90`
- 2 min: `cargo xtask ci could not run fmt/clippy: 'cargo-fmt is not installed' in the minimal rustup profile`
- 3 min: `Desktop app process was reaped when the launching shell exited, so no window or control port remained`
- 10 min: `3 wordcraft-layout tests failed (soft-hyphen break opportunities, ellipse tight wrap) because the container had no Calibri-metric font, only 8 DejaVu files`
- 2 min: `wordcraft --help is treated as a document filename: it opens the GUI and logs '--help: No such file or directory (os error 2)'`
- 2 min: `docs/parity-checklist.md is stale: cargo xtask parity writes 483 of 498 (97.0%) while the committed doc says 482 of 497`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
