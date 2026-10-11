# pydantic-deepagents

**Verdict: runs.** Argusic Score 90 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/vstorm-co/pydantic-deepagents, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/pydantic-deepagents

## Pinned environment

- Project commit: `32b57ba6df24c744537b9b9080394ead6fc02c10`
- Test commit: `32b57ba6df24c744537b9b9080394ead6fc02c10`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 24.7 to 24.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 90 | 5 | 24.7 | 2 | 1 | [run](https://argusic.com/run/561db636-40ed-40be-a3c7-f0e67c8c69bf) |

## What was observed on a clean machine

Attempt 1:

- 12 min: `pydantic-ai-backend 0.2.33 (PyPI latest) removed exports needed by pydantic-deep 0.3.43`
- `14 pre-existing test failures due to pydantic-ai message API changes`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
