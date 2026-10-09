# scientific-agent-skills

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/K-Dense-AI/scientific-agent-skills, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/scientific-agent-skills

## Pinned environment

- Project commit: `92ace75ac21efe19a620434e0ca4e356081fe807`
- Test commit: `92ace75ac21efe19a620434e0ca4e356081fe807`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 16.8 to 16.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 2.5 | 16.8 | 6 | 6 | [run](https://argusic.com/run/0a6cce34-944e-4545-8f81-420efb63a290) |

## What was observed on a clean machine

Attempt 1:

- `System Python 3.12.3 is below pyproject.toml requires-python >=3.13`
- 1 min: `pip install uv failed: externally-managed-environment`
- 0.5 min: `uv sync did not install dev dependency group (pytest, jsonschema, skills-ref)`
- `5 test suites failed in non-isolated mode (cellprofiler, geomaster, relion, scientific-slides, scikit-bio)`
- 0.5 min: `npm install -g uv failed: permissions error`
- `skill_scanner.scan() not directly importable from Python`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
