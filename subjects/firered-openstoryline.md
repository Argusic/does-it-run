# FireRed-OpenStoryline

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/FireRedTeam/FireRed-OpenStoryline, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/firered-openstoryline

## Pinned environment

- Project commit: `c9e945215586f45c12a61c1951ee9a8e9c43a027`
- Test commit: `c9e945215586f45c12a61c1951ee9a8e9c43a027`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 3; wall time 31.3 to 42.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | n/a | 42 | 0 | 0 | [run](https://argusic.com/run/4e392502-3206-456d-b31a-3f43a6f62c12) |
| 1 | pass with mocks | 92 | 45 | 31.3 | 4 | 4 | [run](https://argusic.com/run/98465175-72e3-43c5-8a0f-f9806084d447) |
| 2 | timeout | none | n/a | 42.1 | 0 | 0 | [run](https://argusic.com/run/b49084d1-f2ed-41f1-9c76-67fefc6e50ab) |

## What was observed on a clean machine

Attempt 1:

- 10 min: `langgraph 1.0.10 removed ExecutionInfo from langgraph.runtime, but langgraph-prebuilt 1.0.13 still imports it, breaking langchain.agents import`
- 2 min: `Missing transnetv2-pytorch-weights.pth model weight file`
- 1 min: `Missing resource files (bgms/meta.json, script_templates/meta.json, tts/tts_providers.json, fonts/font_info.json)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
