# browser-use

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/browser-use/browser-use, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/browser-use

## Pinned environment

- Project commit: `fe5ad353091fa2ed5499b94e8fe21094bc2e9e5a`
- Test commit: `fe5ad353091fa2ed5499b94e8fe21094bc2e9e5a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 3; wall time 32.3 to 74.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | 0.5 | 44.2 | 2 | 2 | [run](https://argusic.com/run/e7c7f86c-7663-40da-bacc-dee0e3f0b243) |
| 1 | pass | 100 | 33 | 32.3 | 1 | 1 | [run](https://argusic.com/run/c4ce8f2d-d47f-433b-aa3e-93be2625c0b4) |
| 1 | pass | 100 | 0.15 | 74.7 | 2 | 2 | [run](https://argusic.com/run/f3775baf-a1b3-46f7-a3f3-79104dc23079) |

## What was observed on a clean machine

Attempt 1:

- 0.1 min: `Chromium browser not found - playwright needed to install it`
- `tests/ci/test_search_find.py hangs due to session-scoped http_server fixture conflicting with conftest asyncio fixture scope`

Attempt 1:

- `2 flaky isinstance() type hint tests in test_beta_agent.py fail when run as part of full suite due to import ordering/metaclass identity`

Attempt 1:

- 0.3 min: `Chromium browser not installed - uvx playwright install chromium failed inside the venv due to missing root escalation`
- 10 min: `test_beta_agent.py uses identity checks (isinstance, is) on Generic class annotations imported in different xdist workers, causing failures under --dist=loadscope`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
