# bkmr

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/sysid/bkmr, licensed BSD-3-Clause, written in Rust.

Evidence and recordings: https://argusic.com/subject/bkmr

## Pinned environment

- Project commit: `a6ca05ef4e20baa3c59d96653e8bdf734a27fca1`
- Test commit: `a6ca05ef4e20baa3c59d96653e8bdf734a27fca1`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 11 to 11 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2.5 | 11 | 1 | 1 | [run](https://argusic.com/run/1c68d350-4415-487d-87c0-e520b0aa7b7c) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `Integration tests test_main.rs: two tests (given_debug_flag_when_running_then_enables_debug_mode, given_bookmark_ids_when_showing_then_displays_correct_entries) fail because they invoke the bkmr binary without a database.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
