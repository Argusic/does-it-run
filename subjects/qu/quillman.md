# quillman

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/modal-labs/quillman, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/quillman

## Pinned environment

- Project commit: `7ed27b446538cac92776cd86d5cb8b8ce19ad245`
- Test commit: `7ed27b446538cac92776cd86d5cb8b8ce19ad245`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 11.1 to 11.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 1.14 | 11.1 | 3 | 3 | [run](https://argusic.com/run/12866e46-9a36-4473-af93-0de8d1a22f4b) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Modal cloud token not configured`
- 0.5 min: `sounddevice requires libportaudio (system package)`
- 0.5 min: `No CUDA GPU available for Moshi model inference`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
