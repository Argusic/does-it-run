# parlant

**Verdict: runs with mocks.** Argusic Score 85.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/emcie-co/parlant, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/parlant

## Pinned environment

- Project commit: `ea737442b8ae65854a842542e544fbe7e6144bad`
- Test commit: `ea737442b8ae65854a842542e544fbe7e6144bad`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 23.8 to 23.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 85.33 | 5 | 23.8 | 3 | 2 | [run](https://argusic.com/run/0ab0d769-5312-446c-bcf2-84c7342f6d67) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Missing chromadb module in prepare_migration.py at module level`
- 5 min: `Emcie API key required as default NLP service`
- `parlant CLI (client) cannot import JourneyTriggerUpdateParams from installed parlant-client v3.2.0`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
