# terrapod

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/mattrobinsonsre/terrapod, licensed MPL-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/terrapod

## Pinned environment

- Project commit: `dbc20804c124f37a8a90cd4f18e0e8561a64c5e2`
- Test commit: `dbc20804c124f37a8a90cd4f18e0e8561a64c5e2`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 41.9 to 95.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | 5 | 95.5 | 2 | 2 | [run](https://argusic.com/run/776851f6-e40b-4847-8346-17e970fc68dc) |
| 2 | pass with mocks | 92 | 62 | 41.9 | 3 | 3 | [run](https://argusic.com/run/4ea84d7d-1482-4114-9804-5f80e8c9d406) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Python 3.12 installed but project requires Python >=3.14`
- `No Docker available - cannot run integration tests or build Docker images`

Attempt 2:

- 3 min: `python-hcl2 8.x changed key quoting behavior, breaking module registry tests`
- 2 min: `workspace_rbac_service.py and catalog_rbac_service.py use AuthenticatedUser in runtime annotations but only import under TYPE_CHECKING without from __future__ import annotations`
- 15 min: `Starlette 1.3+ uses _IncludedRouter for include_in_schema=False routes, breaking app.routes iteration in ~120 test assertions`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
