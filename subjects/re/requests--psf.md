# requests

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/psf/requests, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/run/f5b764b0-e8e9-4fbb-b3d9-5213a56a8bfe

## Pinned environment

- Project commit: `611c6162cbc4ac2020a2f91c7cfa4f3abf9bbb60`
- Test commit: `611c6162cbc4ac2020a2f91c7cfa4f3abf9bbb60`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 3.9 to 3.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.5 | 3.9 | 2 | 2 | [run](https://argusic.com/run/f5b764b0-e8e9-4fbb-b3d9-5213a56a8bfe) |

## What was observed on a clean machine

Attempt 1:

- 0.1 min: `python command not found - system only has python3`
- 0.2 min: `externally-managed-environment blocks system-wide pip install`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
