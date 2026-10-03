# nWave

**Verdict: could not verify.** Argusic Score 80 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/nWave-ai/nWave, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/nwave

## Pinned environment

- Project commit: `da401a8384dc867314ba2f4a5fd802fafa593e4f`
- Test commit: `da401a8384dc867314ba2f4a5fd802fafa593e4f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 2; wall time 6.8 to 14.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 6 | 14.4 | 1 | 1 | [run](https://argusic.com/run/c45bae2c-22f0-4243-b359-beda1a2f3d63) |
| 2 | fail | 80 | 8 | 6.8 | 2 | 2 | [run](https://argusic.com/run/839b408f-cf9d-4b50-9ddd-99a61d189d00) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Build failed: lib/python/des not found (force-include target missing)`

Attempt 2:

- 1 min: `pip install failed: externally-managed-environment (PEP 668) blocks system-wide install`
- 2 min: `pip install -e failed: pyproject.toml references lib/python/des which does not exist , DES code is at src/des/`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
