# deep-searcher

**Verdict: runs with mocks.** Argusic Score 56 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/zilliztech/deep-searcher, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/deep-searcher

## Pinned environment

- Project commit: `ddc36db317836bd42302b36f03166bec5324708d`
- Test commit: `ddc36db317836bd42302b36f03166bec5324708d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 0.5 to 4.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 0.5 | 0 | 0 | [run](https://argusic.com/run/65545184-16ca-47b8-ad56-3a0d06176d88) |
| 2 | pass with mocks | 92 | 1.5 | 4.6 | 2 | 2 | [run](https://argusic.com/run/5b21db37-8d31-4fc6-8c9b-e6247a7f1bc7) |

## What was observed on a clean machine

Attempt 2:

- 0.5 min: `XAI LLM test expected default model 'grok-2-latest' but source default was 'grok-4'`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
