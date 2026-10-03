# AI-Youtube-Shorts-Generator

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Anil-matcha/AI-Youtube-Shorts-Generator, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/ai-youtube-shorts-generator

## Pinned environment

- Project commit: `9c7a33e7b927ab650a9b4967ac641649fa05f6d4`
- Test commit: `9c7a33e7b927ab650a9b4967ac641649fa05f6d4`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 3; wall time 10.2 to 17.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 1.2 | 12.2 | 2 | 2 | [run](https://argusic.com/run/4327a267-507e-4887-ae23-c0c4b70acad6) |
| 2 | pass with mocks | 92 | 1 | 17.2 | 1 | 1 | [run](https://argusic.com/run/1166d411-e950-4194-a39d-30cbd0a9e9c9) |
| 3 | pass with mocks | 92 | 0.04 | 10.2 | 0 | 0 | [run](https://argusic.com/run/2bdd5b7e-2117-4993-afb1-14940ae6d27c) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `pip install failed: externally-managed-environment (PEP 668 prevents system-wide install)`
- 5 min: `OpenCV 5 removed CascadeClassifier and bundled haarcascades , local clipper crashed with 'module 'cv2' has no attribute 'CascadeClassifier'`

Attempt 2:

- 2.5 min: `opencv-python 5.0.0 headless lacks cv2.CascadeClassifier needed for face-tracking vertical crop in local clipper`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
