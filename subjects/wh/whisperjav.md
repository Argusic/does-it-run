# WhisperJAV

**Verdict: runs.** Argusic Score 82 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/meizhong986/WhisperJAV, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/whisperjav

## Pinned environment

- Project commit: `982d5dd912f45f928e0237b1d7dfa39c9ee35c15`
- Test commit: `982d5dd912f45f928e0237b1d7dfa39c9ee35c15`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 11 to 39.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 92 | 3 | 11 | 5 | 3 | [run](https://argusic.com/run/68454811-d2a8-4fda-8c2d-1f74b2b80a0b) |
| 2 | pass with mocks | 72 | 5 | 39.4 | 6 | 0 | [run](https://argusic.com/run/0fefb593-c7c0-4a34-9066-db4ba55134f5) |

## What was observed on a clean machine

Attempt 1:

- 0.3 min: `test_legacy.py: stale VAD version assertions (silero -> silero-v3.1)`
- `test_presets.py: asr_config.json restructured in v1.8.9, no longer has 'common_transcriber_options' section`
- `test_acceptance_v1_8_7b0.py: version tests expect 1.8.7b0, actual is 1.9.3 (43 pre-existing failures, 11 errors)`
- `Missing tkinter (system package) blocks test_simple_gap.py, test_tab_spacing.py`
- `Missing PySubtrans (translate extra) blocks 10 tests`

Attempt 2:

- `test_async_cancellation.py: AsyncPipelineManager no longer accepts max_workers kwarg`
- `test_upgrade_cli.py: assumes git branch-based upgrade context`
- `test_install_py_features.py: install.py not structured as importable module with expected attributes`
- `test_update_check_api.py: API response format doesn't match expected keys`
- `tests/config/test_legacy.py: default VAD version changed from silero to silero-v3.1`
- `GUI cannot open window: missing gi/qtpy backends in headless container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
