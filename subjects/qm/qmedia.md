# Qmedia

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/QmiAI/Qmedia, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/qmedia

## Pinned environment

- Project commit: `c890b2543ac5984f2c48789b5191a16374c09083`
- Test commit: `c890b2543ac5984f2c48789b5191a16374c09083`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 20.7 to 38.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 35 | 38.6 | 11 | 11 | [run](https://argusic.com/run/50d85c7a-6304-4240-84d6-faeea07d864a) |
| 2 | pass with mocks | 92 | 20 | 20.7 | 7 | 7 | [run](https://argusic.com/run/d80c6c46-b0b0-43b1-ac4f-7fdd42096ae1) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `PEP 668 externally-managed-environment blocked pip install system-wide`
- 2 min: `NumPy 2.5.4 incompatible with torch 2.2.0 (numpy.long removed)`
- 2 min: `scipy 1.12+ uses np.long incompatible with numpy 1.x`
- 3 min: `transformers 5.20 requires torch>=2.6 but torch 2.2.0 installed`
- 1 min: `python-multipart not installed`
- 1 min: `moviepy 2.x removed moviepy.editor import path`
- 2 min: `FastAPI 0.143 removed add_event_handler`
- 3 min: `faster-whisper model download blocks server at import time`
- 2 min: `PermissionError creating /work/db directory`
- 1 min: `mmrag_server startup crashes when Ollama unavailable`
- `OCR API returns error string for some images causing validation failure`

Attempt 2:

- 1 min: `pip install failed due to externally-managed-environment`
- 2 min: `NumPy 2.x incompatibility with compiled modules`
- 2 min: `Transformers 5.x module import error - nn not defined`
- 1 min: `sentence-transformers 6.x incompatible with transformers 4.45`
- 2 min: `FastAPI add_event_handler removed in 0.165.0`
- 1 min: `moviepy 2.x renamed moviepy.editor import path`
- `Ollama LLM required for full RAG Q&A pipeline`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
