# Jobs_Applier_AI_Agent_AIHawk

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/feder-cr/Jobs_Applier_AI_Agent_AIHawk, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/jobs-applier-ai-agent-aihawk

## Pinned environment

- Project commit: `eb54b9b4f75704ef0106dec17ff0560d97732f9c`
- Test commit: `eb54b9b4f75704ef0106dec17ff0560d97732f9c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 4.4 to 51.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 0.45 | 4.4 | 0 | 0 | [run](https://argusic.com/run/212d759e-a896-4c74-96d4-90bce989fe16) |
| 2 | pass with mocks | 92 | 4 | 51.1 | 2 | 2 | [run](https://argusic.com/run/407996a8-ad6a-4b6c-ae46-43b30ab39e12) |

## What was observed on a clean machine

Attempt 2:

- 38 min: `Invisible-playwright-mcp / Firefox and all 16 bundled plugins install cleanly; the apply flow failed with a generic ExceptionGroup leaving no diagnostics in the TUI`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
