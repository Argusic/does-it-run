# hexstrike-ai

**Verdict: runs.** Argusic Score 94.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/0x4m4/hexstrike-ai, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/hexstrike-ai

## Pinned environment

- Project commit: `d689933ff579d839c676c82b231f8e98326c5f04`
- Test commit: `d689933ff579d839c676c82b231f8e98326c5f04`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 3; wall time 12 to 33.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 31 | 33.8 | 2 | 2 | [run](https://argusic.com/run/5fe66301-0a9b-4a81-8bfd-2060dc754584) |
| 2 | pass with mocks | 92 | 6.2 | 12.3 | 0 | 0 | [run](https://argusic.com/run/69dab2b0-6e22-473a-affd-a23ca623cf11) |
| 3 | pass with mocks | 92 | 10 | 12 | 0 | 0 | [run](https://argusic.com/run/0fe94c01-fd45-41f5-a6f7-814d94a1e615) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `pip3 not installed in base Python`
- 1 min: `PEP 668 externally-managed environment blocked pip install`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
