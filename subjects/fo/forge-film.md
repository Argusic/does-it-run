# forge-film

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/F-R-L/forge-film, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/forge-film

## Pinned environment

- Project commit: `f67f0a003aee58b3afe1b4f48b39ba8db5ed30f0`
- Test commit: `f67f0a003aee58b3afe1b4f48b39ba8db5ed30f0`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 4.8 to 4.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.5 | 4.8 | 2 | 2 | [run](https://argusic.com/run/65b5cfc8-ac3c-4cb7-a406-2726091e3b05) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `forge plan crashed with OpenAIError before mock fallback , _plan() built the LLM provider before checking cfg.llm_api_key, so an empty key caused AsyncOpenAI() to raise Missing credentials`
- 1.5 min: `forge run crashed with same OpenAIError on build_llm_provider() + build_imagegen_provider() , _run() didn't catch provider instantiation exceptions, and build_imagegen_provider() created OpenAIImageGenProvider even with empty key`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
