# qwen-audio-agent

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/QwenAudio/qwen-audio-agent, licensed Apache-2.0, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/qwen-audio-agent

## Pinned environment

- Project commit: `439e81b8c3d09180011b7d3ea2b521472c4f6eac`
- Test commit: `439e81b8c3d09180011b7d3ea2b521472c4f6eac`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 5.1 to 8.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 22 | 8.6 | 0 | 0 | [run](https://argusic.com/run/8a5afbe6-8834-4649-857e-669722cfeb11) |
| 2 | pass with mocks | 92 | 0.8 | 5.1 | 2 | 2 | [run](https://argusic.com/run/0cc93bda-1551-4428-add5-659bddcd21e1) |

## What was observed on a clean machine

Attempt 2:

- 0.3 min: `System Node.js v18.19.1 is below the required v22.22.2 (ENGINES restriction from README)`
- 0.1 min: `Gateway refused to start without DASHSCOPE_API_KEY (mandatory for DashScope realtime voice)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
