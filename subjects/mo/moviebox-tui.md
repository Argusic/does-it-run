# MovieBox-Tui

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/mesamirh/MovieBox-Tui, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/moviebox-tui

## Pinned environment

- Project commit: `cbcc1ae505b3ac6eea4ade704e957467f895df63`
- Test commit: `cbcc1ae505b3ac6eea4ade704e957467f895df63`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 20.8 to 20.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 20 | 20.8 | 1 | 1 | [run](https://argusic.com/run/e3ec8969-91b0-4e98-9804-5bb046778d97) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Three player tests failed due to globally cached LazyLock<Vec<AndroidOpener>> breaking test isolation`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
