# llm-wiki-agent

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/SamurAIGPT/llm-wiki-agent, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/llm-wiki-agent

## Pinned environment

- Project commit: `861c6ecb0a754841da6df635e9ae32d8474275e5`
- Test commit: `861c6ecb0a754841da6df635e9ae32d8474275e5`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 9.2 to 19.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 9.2 | 0 | 0 | [run](https://argusic.com/run/e8650276-cd0a-4c44-bc59-bba93e3271d3) |
| 2 | pass | 100 | 3 | 19.8 | 3 | 3 | [run](https://argusic.com/run/66d6e5d6-0fa0-4611-8c43-757e4c700306) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `Piped wikilinks [[Target|Text]] not resolved , false broken-link warnings on every ingest that uses display text`
- 3 min: `Entity and concept pages created by ingest not added to wiki/index.md`
- 2 min: `update_index() used str.replace so only first entry per section survived`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
