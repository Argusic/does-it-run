# MineContext

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/volcengine/MineContext, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/minecontext

## Pinned environment

- Project commit: `171c7a9ea8091e326ddcf0f10718aa1b58c83c65`
- Test commit: `171c7a9ea8091e326ddcf0f10718aa1b58c83c65`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 17.9 to 17.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 16 | 17.9 | 1 | 1 | [run](https://argusic.com/run/c5b6e048-59a6-4502-86b2-e261f060278e) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `Starlette 1.7.0 changed Jinja2Templates.TemplateResponse API signature to (request, name, context) but route files used the old (name, context) signature, causing TypeError: unhashable type: 'dict'`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
