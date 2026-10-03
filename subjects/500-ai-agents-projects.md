# 500-AI-Agents-Projects

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ashishpatel26/500-AI-Agents-Projects, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/500-ai-agents-projects

## Pinned environment

- Project commit: `9beeb721c2af551bacaab827a76bddaecaa0ca5e`
- Test commit: `9beeb721c2af551bacaab827a76bddaecaa0ca5e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 12 to 12 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 4 | 12 | 6 | 6 | [run](https://argusic.com/run/230540eb-50de-4c61-ba6a-419e3094649b) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `pip install blocked by externally-managed-environment`
- 1 min: `langchain-tavily==0.1.0 version not found in PyPI`
- 2 min: `langchain-core==0.3.0 conflicts with langgraph requiring <0.3`
- 3 min: `CrewAI v1 rejects ChatOpenAI instance for llm parameter`
- 1 min: `Lesson 03 agent.py had missing import os and undefined load_dotenv after patching`
- 0.5 min: `Generated test_shopping.py contained trailing markdown backticks from LLM output`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
