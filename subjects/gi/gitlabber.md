# gitlabber

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ezbz/gitlabber, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/gitlabber

## Pinned environment

- Project commit: `2a015d74b29922b4ddde5f2f4058e261ec1ed142`
- Test commit: `2a015d74b29922b4ddde5f2f4058e261ec1ed142`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 1.5 to 1.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 0.12 | 1.5 | 1 | 1 | [run](https://argusic.com/run/44e52d6c-2dbb-4640-b5c0-dd1ae48d3492) |

## What was observed on a clean machine

Attempt 1:

- 0.1 min: `externally-managed-environment (PEP 668) prevents system-wide pip install`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
