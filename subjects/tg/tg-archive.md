# tg-archive

**Verdict: runs with mocks.** Argusic Score 56 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/knadh/tg-archive, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/tg-archive

## Pinned environment

- Project commit: `b8f3febaad1180cd581bed0ff07d582d012e8c0b`
- Test commit: `b8f3febaad1180cd581bed0ff07d582d012e8c0b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 8 to 13.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 13.6 | 0 | 0 | [run](https://argusic.com/run/2cde3eb8-971f-4172-9834-c6def8006369) |
| 2 | pass with mocks | 92 | 7 | 8 | 1 | 1 | [run](https://argusic.com/run/4d859a83-b40a-4771-a27f-17bd88a615dd) |

## What was observed on a clean machine

Attempt 2:

- 6 min: `ImportError: failed to find libmagic when running tg-archive --build (system libmagic.so.1 missing; no root to apt install)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
