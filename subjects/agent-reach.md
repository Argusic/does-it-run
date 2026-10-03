# Agent-Reach

**Verdict: runs.** Argusic Score 97.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Panniantong/Agent-Reach, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/agent-reach

## Pinned environment

- Project commit: `06c202b03400a7d31886bf4399213706da1a0324`
- Test commit: `06c202b03400a7d31886bf4399213706da1a0324`
- Worker image digests: `sha256:33ceb71981b602c1a7443a53469e4dba065f7503eab3078a2d7a57a2ab987517`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 3; wall time 2.4 to 7.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1.63 | 7.5 | 0 | 0 | [run](https://argusic.com/run/cd70c5bd-065a-4631-8816-747f82f301ef) |
| 2 | pass | 100 | 0.25 | 2.5 | 0 | 0 | [run](https://argusic.com/run/d8315dc6-730a-4b62-89a9-3bdb590b3d81) |
| 3 | pass with mocks | 92 | 0.5 | 2.4 | 0 | 0 | [run](https://argusic.com/run/b4831858-dd14-4125-8084-a743e4186e8d) |

## What was observed on a clean machine

No error was recorded during the valid runs.

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
