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
- Valid runs: 2; wall time 14.4 to 18.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 17.4 | 18.7 | 6 | 6 | [run](https://argusic.com/run/30d1c276-fa70-488c-911e-b8cfcaff9815) |
| 2 | pass with mocks | 92 | 3 | 14.4 | 5 | 5 | [run](https://argusic.com/run/15d879f0-fe3a-49b4-aada-1b33f965336a) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `uv package manager not pre-installed`
- 1 min: `'source' not available in sh, can't activate venv`
- 1 min: `.env file loaded by pydantic-settings but os.getenv() at module init time does not read it`
- 1 min: `Default SHORT_TERM_MEMORY_DB_PATH=/app/data/memory.db not writable outside Docker`
- 2 min: `'fastapi run' command fails with ModuleNotFoundError due to import path resolution`
- `Mock Groq/ElevenLabs/Together/Qdrant API keys cause 401/connection errors on POST`

Attempt 2:

- 1 min: `langchain v1.2 removed langchain.prompts module; import PromptTemplate from langchain_core.prompts`
- 2 min: `mcp 1.12+ incompatible with pydantic 2.10 (chainlit dep chain)`
- 1 min: `scipy 1.18 uses np.long which was removed in numpy 2.x`
- 2 min: `chainlit 2.x renamed AudioChunk and broke API; code expects chainlit 1.x`
- 1 min: `starlette 1.x removed on_startup kwarg from Router; fastapi 0.115 needs starlette<1`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
