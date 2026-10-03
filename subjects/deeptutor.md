# DeepTutor

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/HKUDS/DeepTutor, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/deeptutor

## Pinned environment

- Project commit: `a053fecf6eeca51ded680de8b8fc41ef63857b11`
- Test commit: `a053fecf6eeca51ded680de8b8fc41ef63857b11`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 55.9 to 55.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 4.5 | 55.9 | 7 | 7 | [run](https://argusic.com/run/542e86ae-c955-492c-8102-83c7ddf0b9f3) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `Missing slack_sdk dependency for partner channels`
- 0.5 min: `Missing python-telegram-bot dependency for partner channels`
- 0.5 min: `Missing matrix-nio dependency for partner channels`
- 0.5 min: `Missing slackify_markdown dependency for partner channels`
- 5 min: `FastAPI 0.141.x _IncludedRouter breaks test route introspection via app.routes`
- 1 min: `Sandbox runner test uses python but only python3 exists in container`
- 1 min: `Missing lark-oapi dependency for Feishu partner channels`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
