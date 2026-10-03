# humanize-text

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/lynote-ai/humanize-text, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/humanize-text

## Pinned environment

- Project commit: `79bb396acfc349bf600ec1619106b059939ff236`
- Test commit: `79bb396acfc349bf600ec1619106b059939ff236`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 10.3 to 10.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 1.5 | 10.3 | 2 | 2 | [run](https://argusic.com/run/a2f775de-44c1-414c-aca4-e8cea783ac80) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `pip install fails due to externally-managed-environment (PEP 668) in container`
- 1 min: `test_openrouter_provider failed because pre-existing OPENROUTER_API_KEY env var overrode test config value per code design`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
