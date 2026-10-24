# soundcraft

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/storytold/soundcraft, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/soundcraft

## Pinned environment

- Project commit: `52471b37e957feaea56dfd48932ef16d314cc74a`
- Test commit: `52471b37e957feaea56dfd48932ef16d314cc74a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 26.8 to 60.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 60.7 | 0 | 0 | [run](https://argusic.com/run/555cd57f-3e19-4fb4-b98f-24d57479e085) |
| 2 | pass | 100 | 24 | 26.8 | 4 | 4 | [run](https://argusic.com/run/28cebcff-6cca-47d8-8343-6d8b7241826d) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `Rust toolchain not installed (no rustc found)`
- 1 min: `ALSA .pc file missing (libasound2-dev not installed)`
- 1 min: `Linker cannot find -lasound (only .so.2 symlink exists, no .so)`
- 15 min: `dependabot bumped 4 deps (symphonia 0.5.5->0.6.1, cpal 0.16.0->0.18.2, egui/eframe/egui_kittest 0.36.2->0.37.0) without updating code - 76+ compilation errors`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
