# Gito

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Nayjest/Gito, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/gito

## Pinned environment

- Project commit: `f48498d192ede9aa81808c2579c69cc5d7919e20`
- Test commit: `f48498d192ede9aa81808c2579c69cc5d7919e20`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 2 to 3.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 2 | 1 | 1 | [run](https://argusic.com/run/2cb9f130-5637-4744-9ffd-e6f6754a501f) |
| 2 | pass | 100 | 4 | 3.4 | 1 | 1 | [run](https://argusic.com/run/09d45d09-cc08-4766-ada7-fc3b7a1a509d) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `tests/test_version.py hardcoded 'python' but only python3 is on PATH in this container`

Attempt 2:

- 1 min: `tests/test_version.py: subprocess.run(['python', ...]) fails because 'python' not on PATH in venv`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
