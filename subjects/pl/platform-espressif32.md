# platform-espressif32

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/platformio/platform-espressif32, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/platform-espressif32

## Pinned environment

- Project commit: `1152c8f69146ca0c20ab772264606b3cc61ec67c`
- Test commit: `1152c8f69146ca0c20ab772264606b3cc61ec67c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 5.9 to 13.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 6 | 5.9 | 0 | 0 | [run](https://argusic.com/run/c495be1d-2a6d-49a4-b52b-865d849775e4) |
| 2 | pass | 100 | 28 | 13.6 | 1 | 1 | [run](https://argusic.com/run/b4bbef2c-ea86-47c6-a59e-91f40b059a1c) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `pip3 install failed due to externally-managed-environment (PEP 668)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
