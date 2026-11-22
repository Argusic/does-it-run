# sleepless-agent

**Verdict: runs with mocks.** Argusic Score 87 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/context-machine-lab/sleepless-agent, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/sleepless-agent

## Pinned environment

- Project commit: `dbeb1c28699bfc7af48687203a2baa06c62cf7a1`
- Test commit: `dbeb1c28699bfc7af48687203a2baa06c62cf7a1`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 2.7 to 52.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 51 | 52.7 | 3 | 3 | [run](https://argusic.com/run/3dcf8fa6-b95b-4c89-a954-5794a2f3373d) |
| 2 | pass with mocks | 82 | 0.5 | 2.7 | 2 | 1 | [run](https://argusic.com/run/c79c0665-bb3a-4b1f-ac04-96492504aeae) |

## What was observed on a clean machine

Attempt 1:

- 20 min: `daemon hard-requires SLACK_BOT_TOKEN/SLACK_APP_TOKEN despite README promising CLI-only mode (RuntimeError in SleeplessAgent.__init__)`

Attempt 2:

- `Makefile test command references non-existent module 'sleepless_agent.runtime'`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
