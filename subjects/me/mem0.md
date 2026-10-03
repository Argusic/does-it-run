# mem0

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/mem0ai/mem0, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/mem0

## Pinned environment

- Project commit: `8d6c001966573786d36908bfe4dfd52935749200`
- Test commit: `8d6c001966573786d36908bfe4dfd52935749200`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 49.4 to 49.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 12 | 49.4 | 4 | 4 | [run](https://argusic.com/run/fe5f8de5-eef7-4af0-a453-8cb691b463b8) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `test_main.py OOM-killed (exit 137) with MEM0_TELEMETRY=True due to torch import from telemetry chain`
- 2 min: `httpx proxy URL pattern validation rejects bare scheme keys`
- 1 min: `test_notices.py and test_oss_to_platform_migrate.py need MEM0_TELEMETRY=True but default is False`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
