# posting

**Verdict: runs.** Argusic Score 96.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/darrenburns/posting, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/posting

## Pinned environment

- Project commit: `56703a11513e8e74e681b4f859f31945b71e746f`
- Test commit: `56703a11513e8e74e681b4f859f31945b71e746f`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 3; wall time 16.6 to 30.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 17 | 16.6 | 2 | 2 | [run](https://argusic.com/run/f9cc91c3-57d9-4167-9738-fa0d6d3232ea) |
| 2 | pass | 90 | 0.5 | 20.8 | 2 | 1 | [run](https://argusic.com/run/741b1598-1c8d-4061-96cd-74fce4ed132a) |
| 3 | pass | 100 | 35 | 30.8 | 3 | 3 | [run](https://argusic.com/run/ea79ea42-3e3f-453f-8135-07be31e885b4) |

## What was observed on a clean machine

Attempt 1:

- 10 min: `textual/filter.py: monochrome_style() crashes on None style (AttributeError: 'NoneType' object has no attribute 'color')`
- 2 min: `59 snapshot mismatches in test_snapshots.py`

Attempt 2:

- `8 snapshot comparison mismatches: test environment renders UI slightly differently than snapshot origin (expected for snapshot tests in new env)`
- `TestConfig::test_config crashes with AttributeError when NO_COLOR=1 (textual monochrome filter bug with null style segments)`

Attempt 3:

- 5 min: `NO_COLOR=1 env var crashes Textual 6.1.0 monochrome filter when segments have style=None (AttributeError: 'NoneType' object has no attribute 'color')`
- 2 min: `Watchfiles Rust inotify watcher fails with 'Too many open files (os error 24)' due to low inotify max_user_instances (128) in container`
- 8 min: `13 snapshot tests fail in parallel mode (-n 24) due to race conditions; no failures in serial mode`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
