# Fyrox

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/FyroxEngine/Fyrox, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/fyrox

## Pinned environment

- Project commit: `dc354e0d98279dbf84cbbd1a8cd3672501ccfbbc`
- Test commit: `dc354e0d98279dbf84cbbd1a8cd3672501ccfbbc`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 19.5 to 53.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 10.2 | 19.5 | 2 | 2 | [run](https://argusic.com/run/d4b48f26-74bc-4b0f-87de-02e01746373e) |
| 2 | pass | 100 | 45 | 53.5 | 5 | 5 | [run](https://argusic.com/run/405de831-8684-479b-900d-2144453950ba) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `alsa-sys build failed: system libasound2-dev package not installed`
- 0.5 min: `fyrox-core-derive test 'doc_comments' failed: doc comment format changed in Rust 1.98 (multiline doc strings now include literal newlines)`

Attempt 2:

- 2 min: `Rust toolchain not installed`
- 3 min: `ALSA dev headers (libasound2-dev) not available - no root access`
- 3 min: `fyrox-core-derive doc_comment test failed on Rust 1.99.1 - multiline doc comments preserve newlines`
- 2 min: `Disk full during test build (40GB overlay at 100%)`
- 1 min: `Template generator added test_project to workspace Cargo.toml`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
