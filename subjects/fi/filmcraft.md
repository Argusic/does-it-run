# filmcraft

**Verdict: runs.** Argusic Score 90 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/storytold/filmcraft, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/filmcraft

## Pinned environment

- Project commit: `ada55eb62568ba75be25cd12bd07b5fbdc37f88d`
- Test commit: `ada55eb62568ba75be25cd12bd07b5fbdc37f88d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 65.1 to 87 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | n/a | 87 | 0 | 0 | [run](https://argusic.com/run/54a890f6-7b86-4126-83e7-7d4fd3f3b4b4) |
| 2 | pass | 90 | 42 | 65.1 | 4 | 2 | [run](https://argusic.com/run/e7def6f7-a2fd-4173-99c7-6329871e8128) |

## What was observed on a clean machine

Attempt 2:

- 5 min: `Missing libasound2-dev (ALSA headers/pkg-config file) required by alsa-sys build script`
- `Test failure: filmcraft-matroska mjpeg_ac3 , duration mismatch between ffprobe and decoder (pre-existing)`
- `Test failure: engine shortcuts_tests::assign_reassigns_conflicts_and_undoes (pre-existing)`
- `40 GB disk fills during full workspace test+release build`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
