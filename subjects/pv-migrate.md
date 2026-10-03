# pv-migrate

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/utkuozdemir/pv-migrate, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/pv-migrate

## Pinned environment

- Project commit: `78c984e2fb858b785ecb93d36cc4d2626f847108`
- Test commit: `78c984e2fb858b785ecb93d36cc4d2626f847108`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 16.6 to 16.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 17 | 16.6 | 1 | 1 | [run](https://argusic.com/run/f67389ed-2652-4fb8-8522-9d316d12b2ee) |

## What was observed on a clean machine

Attempt 1:

- 10 min: `Go compiler not pre-installed in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
