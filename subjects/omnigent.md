# omnigent

**Verdict: runs.** Argusic Score 97.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/omnigent-ai/omnigent, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/omnigent

## Pinned environment

- Project commit: `197dab25cd2e892016e3d22a36aad7a1ae63ec54`
- Test commit: `197dab25cd2e892016e3d22a36aad7a1ae63ec54`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 3; wall time 14.4 to 33.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 27 | 33.4 | 4 | 4 | [run](https://argusic.com/run/328cc80f-65ea-4826-ba61-12cf9daed482) |
| 2 | pass | 100 | 2.5 | 14.4 | 5 | 5 | [run](https://argusic.com/run/b29fb689-43e5-4ebb-801a-239bbed90ce2) |
| 3 | pass | 100 | 2 | 28 | 4 | 4 | [run](https://argusic.com/run/1ac0e43e-3e35-43d0-af2e-a4a86c05ecd7) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node.js 18.19.1 too old for web UI build (requires >=22.13.0); web UI skipped`
- 1 min: `PEP 668 externally managed Python blocks system-wide pip install`
- 1 min: `uv sync --all-extras has incompatible extras antigravity/cwsandbox`
- 1 min: `No uv or pnpm pre-installed`

Attempt 2:

- 1.5 min: `System Node.js 18.19.1 below minimum 22.13.0; web UI build skipped`
- 0.5 min: `tests/inner/test_databricks_executor.py: No module named 'databricks'`
- 0.5 min: `tests/runtime/test_telemetry.py: No module named 'opentelemetry.sdk'`
- 0.1 min: `tests/test_subpackage_legal_files.py: No module named 'scripts.build_subpackages'`
- `2 flaky crash_handler tests (file-rotation race) failed`

Attempt 3:

- 1 min: `Node.js 18.19.1 too old (need 22.13+)`
- 0.5 min: `scripts/__init__.py missing (test import error)`
- `test_render_tty_shows_header_and_copyable_path fails in container (NO_COLOR=1 + TERM=dumb)`
- `3 PostgreSQL tests fail (psycopg not installed)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
