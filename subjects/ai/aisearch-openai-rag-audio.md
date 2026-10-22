# aisearch-openai-rag-audio

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Azure-Samples/aisearch-openai-rag-audio, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/aisearch-openai-rag-audio

## Pinned environment

- Project commit: `85d0b4e25dc7cd4c601dc789450690b073577afc`
- Test commit: `85d0b4e25dc7cd4c601dc789450690b073577afc`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 3.4 to 3.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 3 | 3.4 | 3 | 3 | [run](https://argusic.com/run/bc4b78a2-066a-4d9b-abe8-55443da51409) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `requirements.txt was UTF-16-LE encoded with BOM, causing pip to fail`
- 0.5 min: `pyproject.toml ruff target-version set to py39 but code uses Python 3.10+ match statements`
- 0.5 min: `type(self.text) == str flagged by Ruff E721`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
