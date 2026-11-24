# shotgun

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/shotgun-sh/shotgun, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/shotgun

## Pinned environment

- Project commit: `4d344d5a46aafc815de441ff670d4131187f33e6`
- Test commit: `4d344d5a46aafc815de441ff670d4131187f33e6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 52.1 to 55.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1 | 55.3 | 3 | 3 | [run](https://argusic.com/run/86118c2a-2ace-4f69-b6e0-72f9cabdee79) |
| 2 | pass | 100 | 3 | 52.1 | 2 | 2 | [run](https://argusic.com/run/cff33536-6d47-42a2-aaec-2475524809a3) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `OPENROUTER_API_KEY env var caused test_provider.py 3 failures`
- 5 min: `OPENROUTER_API_KEY caused test_streaming_detection.py 3 failures`
- 3 min: `OPENROUTER_API_KEY caused test_config_manager.py 2 failures`

Attempt 2:

- 5 min: `OPENROUTER_API_KEY env var in harness contaminated provider-selection tests in test_config_manager.py`
- 2 min: `Missing trio package for anyio trio backend tests in test_compaction.py and test_welcome_message.py`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
