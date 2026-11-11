# reverse-api-engineer

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/kalil0321/reverse-api-engineer, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/reverse-api-engineer

## Pinned environment

- Project commit: `ab9919b652eca1c7b323c3f7c7b37ded3cef12a0`
- Test commit: `ab9919b652eca1c7b323c3f7c7b37ded3cef12a0`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 1.5 to 7.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 2 | 1.5 | 0 | 0 | [run](https://argusic.com/run/c0c36e59-9829-48c5-a2c4-74cb47e1f94d) |
| 2 | pass | 100 | 1 | 7.4 | 2 | 2 | [run](https://argusic.com/run/22055369-6c64-4368-983a-45fe86e5625e) |

## What was observed on a clean machine

Attempt 2:

- 3 min: `test_cli_no_httpx.py: python3 -I skips user site-packages where httpx2 is installed`
- 2 min: `test_cli_followups.py: uses 'uv run' which is not available`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
