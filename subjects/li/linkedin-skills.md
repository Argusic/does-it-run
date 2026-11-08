# linkedin-skills

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/sergebulaev/linkedin-skills, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/linkedin-skills

## Pinned environment

- Project commit: `14d332b9e91e314f2e35b299246ced6df2594fab`
- Test commit: `14d332b9e91e314f2e35b299246ced6df2594fab`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 1.4 to 3.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 3.5 | 3.7 | 1 | 1 | [run](https://argusic.com/run/05402c8c-e39e-4b63-b773-edf5822e3b05) |
| 2 | pass with mocks | 92 | 3.2 | 1.4 | 1 | 1 | [run](https://argusic.com/run/3e5ae49a-5b57-4ee3-a7ad-df9934a00cb6) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `pip install failed , externally-managed-environment (PEP 668)`

Attempt 2:

- 0.5 min: `Missing PyYAML dependency needed by test suite for YAML frontmatter parsing`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
