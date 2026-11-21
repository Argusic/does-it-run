# sample-strands-agent-with-agentcore

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/aws-samples/sample-strands-agent-with-agentcore, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/sample-strands-agent-with-agentcore

## Pinned environment

- Project commit: `05269cb40a2f2c5aa331965b332c6480d95dce06`
- Test commit: `05269cb40a2f2c5aa331965b332c6480d95dce06`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 6.4 to 6.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 4 | 6.4 | 4 | 4 | [run](https://argusic.com/run/74dc10cc-9948-42ec-a5b3-b1ccc4dcf31a) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `strands_tools.calculator was removed in strands-agents-tools v0.9.0, causing ImportError in src/agents/chat_agent.py`
- 2 min: `strands_tools.shell was removed in strands-agents-tools v0.9.0, causing ImportError in src/skill/skill_tools.py`
- 1 min: `builtin_tools lazy import for nova_act raised ModuleNotFoundError on app startup`
- `Next.js 16 requires Node >=20.9.0; container has Node 18.19.1 , frontend cannot be built or tested`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
