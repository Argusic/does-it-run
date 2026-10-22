# chatgpt-video-editing-skills

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Jaycheng1103/chatgpt-video-editing-skills, licensed MIT, written in Shell.

Evidence and recordings: https://argusic.com/subject/chatgpt-video-editing-skills

## Pinned environment

- Project commit: `dc2f10ac4616603188aff3df9ea6548a8da36355`
- Test commit: `dc2f10ac4616603188aff3df9ea6548a8da36355`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 3.8 to 3.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 3 | 3.8 | 7 | 7 | [run](https://argusic.com/run/e2b195fe-0051-4772-81f0-bb6c5c259116) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `system Node.js v18 does not meet npx skills requirement (>=22.20.0)`
- 1 min: `uv (Python package manager) not found`
- `pip install failed due to externally-managed-environment`
- 2 min: `ELEVENLABS_API_KEY not available`
- `render EDL used segments key but render.py expects ranges key`
- 1 min: `loudnorm audio normalization failed on silent test video (I=-inf)`
- 1 min: `transcribe refused silent track 0 (peak -inf dBFS)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
