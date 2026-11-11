# MovieBox-Tui

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/mesamirh/MovieBox-Tui, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/moviebox-tui

## Pinned environment

- Project commit: `cbcc1ae505b3ac6eea4ade704e957467f895df63`
- Test commit: `cbcc1ae505b3ac6eea4ade704e957467f895df63`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 12.6 to 20.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 20 | 20.8 | 1 | 1 | [run](https://argusic.com/run/e3ec8969-91b0-4e98-9804-5bb046778d97) |
| 2 | pass with mocks | 92 | 4 | 12.6 | 1 | 1 | [run](https://argusic.com/run/17e3d72c-e36c-4aae-9ab9-fd79b6862f71) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Three player tests failed due to globally cached LazyLock<Vec<AndroidOpener>> breaking test isolation`

Attempt 2:

- 2 min: `3 test failures in player::tests: test_android_intent_commands_fallback_order, test_detect_prioritizes_android_intent_on_termux, test_has_graphical_display_detection. Root cause: ANDROID_OPENERS static LazyLock cached globally, tests creati`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
