# video-use

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/browser-use/video-use, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/video-use

## Pinned environment

- Project commit: `b877063835e6ea6e457124da7e28a0ae26691dc3`
- Test commit: `b877063835e6ea6e457124da7e28a0ae26691dc3`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 8 to 8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 8 | 8 | 3 | 3 | [run](https://argusic.com/run/08e6ec35-9556-466f-89b5-c57d68fa4084) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `pip install -e . failed: externally-managed-environment (Debian PEP 668)`
- 1 min: `pytest module not found`
- 2 min: `timeline_view.py extract_frames fails when frame timestamp >= video duration`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
