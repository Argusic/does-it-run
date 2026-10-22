# AutoHarness

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/aiming-lab/AutoHarness, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/run/59a82b04-3af1-4c2d-97e8-78607adfc00f

## Pinned environment

- Project commit: `3561e468f9ca9f9bf282512e695bd32e4e90fef4`
- Test commit: `3561e468f9ca9f9bf282512e695bd32e4e90fef4`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 4.9 to 4.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 4.9 | 3 | 3 | [run](https://argusic.com/run/59a82b04-3af1-4c2d-97e8-78607adfc00f) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `System pip refused install: PEP 668 externally-managed environment`
- 1 min: `pytest not installed in fresh venv`
- 1 min: `test_cli_wrap test_wrap_failing_command failed: 'python' not found on PATH in this container (only python3 exists), exit 127 instead of 42`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
