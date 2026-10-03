# spec-kitty

**Verdict: could not verify.** Argusic Score 73.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/spec-kitty/spec-kitty, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/spec-kitty

## Pinned environment

- Project commit: `bcb7fe37669ef93f45b21bb08f10faf9032b5c04`
- Test commits: `614c52cb382d6bbd4ae8d4daab060320502fc14c`, `bcb7fe37669ef93f45b21bb08f10faf9032b5c04`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, no run possible
- Valid runs: 4; wall time 10.7 to 87.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 15 | 84.2 | 5 | 5 | [run](https://argusic.com/run/071aa891-96e3-448f-ae93-5c0de6cc0012) |
| 1 | fail | 20 | n/a | 10.7 | 0 | 0 | [run](https://argusic.com/run/2eefbe57-9a73-41f6-be14-2fd6b1634433) |
| 2 | timeout | none | n/a | 87.4 | 0 | 0 | [run](https://argusic.com/run/3042cd86-148f-4bf6-906f-1e8b70862c95) |
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
