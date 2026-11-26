# ung220z-tool

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Hut-hzf/ung220z-tool, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/ung220z-tool

## Pinned environment

- Project commit: `4eb1b1f7a7a2eef59820dea5ae91c70da4b2c4f9`
- Test commit: `4eb1b1f7a7a2eef59820dea5ae91c70da4b2c4f9`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 2.6 to 5.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 0.9 | 5.8 | 1 | 1 | [run](https://argusic.com/run/ba122a3e-86f5-4df3-a393-ed6fc96f324f) |
| 2 | pass with mocks | 92 | 3 | 2.6 | 1 | 1 | [run](https://argusic.com/run/5b7fa5db-25e9-4c3b-88c1-f248b45f5dac) |

## What was observed on a clean machine

Attempt 1:

- 0.1 min: `Missing python3-cryptography module (required by ontkit/zte_factory.py for AES-ECB operations)`

Attempt 2:

- 2 min: `ontkit/zte_factory.py requires 'cryptography' package, but README claims 'standard library only'`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
