# spec-kitty

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Priivacy-ai/spec-kitty, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/run/071aa891-96e3-448f-ae93-5c0de6cc0012

## Pinned environment

- Project commit: `614c52cb382d6bbd4ae8d4daab060320502fc14c`
- Test commit: `614c52cb382d6bbd4ae8d4daab060320502fc14c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 82.3 to 84.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 15 | 84.2 | 5 | 5 | [run](https://argusic.com/run/071aa891-96e3-448f-ae93-5c0de6cc0012) |
| 2 | pass | 100 | 0.17 | 82.3 | 1 | 1 | [run](https://argusic.com/run/8d916f4c-e4e8-4ddf-bd6e-9471c2b05cf1) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `pip install in externally managed environment required venv creation`
- 1 min: `typer 0.27.2 broke click.Group isinstance check (TyperGroup no longer extends click.Group)`
- `5 golden-help-fixture tests fail due to click/typer tooltip text format changes`
- `12 setup_plan_phases tests error due to missing git commit sha in shallow clone`
- `xdist --dist loadfile KeyError with WorkerController race`

Attempt 2:

- 3.3 min: `mypy not installed (test dependency gap)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
