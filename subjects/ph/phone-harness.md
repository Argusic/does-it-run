# phone-harness

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ShawnPana/phone-harness, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/phone-harness

## Pinned environment

- Project commit: `68d883f7dc40612cb638c849d6302cd8707ab7c7`
- Test commit: `68d883f7dc40612cb638c849d6302cd8707ab7c7`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 5.2 to 5.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 0.5 | 5.2 | 1 | 1 | [run](https://argusic.com/run/f29e2c54-52ac-4453-8559-7dd5e372177c) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `System python3.12 is externally-managed; pip install would fail without a venv`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
