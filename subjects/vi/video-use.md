# video-use

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/browser-use/video-use, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/video-use

## Pinned environment

- Project commit: `b877063835e6ea6e457124da7e28a0ae26691dc3`
- Test commit: `b877063835e6ea6e457124da7e28a0ae26691dc3`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 4.7 to 8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 8 | 8 | 3 | 3 | [run](https://argusic.com/run/08e6ec35-9556-466f-89b5-c57d68fa4084) |
| 2 | pass | 100 | 0.5 | 4.7 | 1 | 1 | [run](https://argusic.com/run/6c18c722-1d02-4f25-ab12-45cf8c0d3a31) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `pip install -e . failed: externally-managed-environment (Debian PEP 668)`
- 1 min: `pytest module not found`
- 2 min: `timeline_view.py extract_frames fails when frame timestamp >= video duration`

Attempt 2:

- 0.3 min: `extract_frames fails when end=video duration , ffmpeg produces no frame at the last timeslice`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
