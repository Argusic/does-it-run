# ava-whatsapp-agent-course

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/neural-maze/ava-whatsapp-agent-course, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/ava-whatsapp-agent-course

## Pinned environment

- Project commit: `338fd6870df9097165fceb3bbfc3cb0c95e584cd`
- Test commit: `338fd6870df9097165fceb3bbfc3cb0c95e584cd`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 18.7 to 18.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 17.4 | 18.7 | 6 | 6 | [run](https://argusic.com/run/30d1c276-fa70-488c-911e-b8cfcaff9815) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `uv package manager not pre-installed`
- 1 min: `'source' not available in sh, can't activate venv`
- 1 min: `.env file loaded by pydantic-settings but os.getenv() at module init time does not read it`
- 1 min: `Default SHORT_TERM_MEMORY_DB_PATH=/app/data/memory.db not writable outside Docker`
- 2 min: `'fastapi run' command fails with ModuleNotFoundError due to import path resolution`
- `Mock Groq/ElevenLabs/Together/Qdrant API keys cause 401/connection errors on POST`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
