# builder

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/frappe/builder, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/builder

## Pinned environment

- Project commit: `4eea9c52b7908c9466e01a28b68d1e39e6c8e22b`
- Test commit: `4eea9c52b7908c9466e01a28b68d1e39e6c8e22b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 16.7 to 16.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 16 | 16.7 | 7 | 7 | [run](https://argusic.com/run/5b4019e6-dcc0-4c3a-b941-a05cda1fe014) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node.js v18.19.1 is too old (requires >=20.19.0)`
- 1 min: `Yarn not installed`
- 1 min: `frappe-ui git submodule not initialized`
- 1 min: `Yarn install blocked by engine check (eslint 10 requires Node ^20.19.0 || ^22.13.0)`
- 2 min: `Frontend vitest tests fail: ReferenceError: window is not defined in translation.ts`
- 5 min: `Frappe framework cannot be pip-installed: requires mysqlclient (pkg-config not found)`
- 2 min: `Backend Python tests needing real DB (test_locks, test_read_page, test_run_python, test_attach_script, test_get_document, test_attached_images, test_page_settings, test_edit_component, test_cache_markers, test_pending, test_web) fail with f`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
