# devops-ai-guidelines

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/VersusControl/devops-ai-guidelines, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/devops-ai-guidelines

## Pinned environment

- Project commit: `e01855ec61afd46542e6550c0922834ff3c578c7`
- Test commit: `e01855ec61afd46542e6550c0922834ff3c578c7`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 2.9 to 5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 2 | 5 | 0 | 0 | [run](https://argusic.com/run/ed8bc44d-80d7-401a-978f-bb69b087b0ba) |
| 2 | pass with mocks | 92 | 0.5 | 2.9 | 2 | 2 | [run](https://argusic.com/run/abe1f593-5df8-4ebd-b047-f050d273f406) |

## What was observed on a clean machine

Attempt 2:

- 3 min: `03-ai-agent-for-devops/code/07/tests/test_basic.py had sys.path pointing at src/ instead of project root, breaking relative imports in tools/log_reader.py (from ..config import Config)`
- 1 min: `System Python3 is externally-managed (PEP 668), preventing pip install system-wide`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
