# social-account-doctor

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/JuneYaooo/social-account-doctor, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/social-account-doctor

## Pinned environment

- Project commit: `2438d5ae7c8e7d876ac89b5e621980fa50a5e0dd`
- Test commit: `2438d5ae7c8e7d876ac89b5e621980fa50a5e0dd`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 6.5 to 6.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 7 | 6.5 | 1 | 1 | [run](https://argusic.com/run/052759c9-1033-4896-9033-e8953a7bd297) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `requests package missing from requirements.txt but required by analyze_image.py and ocr_screenshot.py`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
