# iocraft

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ccbrown/iocraft, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/iocraft

## Pinned environment

- Project commit: `7eae7583da91c2d907c2b0389349cb34525012e4`
- Test commit: `7eae7583da91c2d907c2b0389349cb34525012e4`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 26.5 to 26.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8 | 26.5 | 1 | 1 | [run](https://argusic.com/run/700077d1-a847-430e-839b-928a760c609b) |

## What was observed on a clean machine

Attempt 1:

- `NO_COLOR=1 environment variable set in container suppresses all SGR color output, causing 4 tests (color::background_sgr_matches_expected, color::foreground_sgr_matches_expected, backend::crossterm::test_fullscreen_diff_styled_text_preserve`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
