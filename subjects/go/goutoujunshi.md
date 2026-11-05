# goutoujunshi

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/shengjidaguai-china/goutoujunshi, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/goutoujunshi

## Pinned environment

- Project commit: `6db7354a4002dc7c448a9c87ffdad8132570c9d3`
- Test commit: `6db7354a4002dc7c448a9c87ffdad8132570c9d3`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 3.3 to 5.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 0.01 | 5.1 | 0 | 0 | [run](https://argusic.com/run/35852230-95e6-4947-b07d-e8a632793b44) |
| 2 | pass | 100 | 3 | 3.3 | 0 | 0 | [run](https://argusic.com/run/42560ac5-1a54-4c80-b291-4a510ee10d6d) |

## What was observed on a clean machine

No error was recorded during the valid runs.

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
